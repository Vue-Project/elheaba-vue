<template>
	<div class="lock-screen bg-g1">
		<div class="lock-form">
			Enter Password
			<form  class="form-group" :action="redirectPath" method="GET">
				<!-- <label for="form_name">Name</label> -->
				<input type="password" name="_pw" class="form-control" placeholder="Your Password"
					required="required" data-error="Password is required.">
					<!-- <input type="submit" class="btn btn-unlock" value="UnLock"/> -->
					<button class="btn btn-unlock" type="submit">
            UnLock
          </button>
			</form >

			
		</div>
	</div>
</template>

<script>
export default {
  data: function() {
    return {
      methodLoginValue: '',
      isAuthorised: false
    }
  },
  computed: {
    redirectPath() {
      const path = this.$route.query.previousPath
      return path || this.$router.push({ path: '/' })// this.localePath('/') 
    }
  },
  mounted() {
    this.isAuthorised = this.$passwordProtect.isAuthorised()
  },
  methods: {
    loginUser() {
      this.$passwordProtect.authorise(this.methodLoginValue)
      this.isAuthorised = this.$passwordProtect.isAuthorised()
      this.$router.push(this.redirectPath)
    },
    removeAuthorisation() {
      this.$passwordProtect.removeAuthorisation()
      this.isAuthorised = this.$passwordProtect.isAuthorised()
    }
  }
}
</script>

<style>


.lock-form{
	width: 350px;
	color: #ffffff;
	position: relative;
}

.btn-unlock{
	position: absolute;
	bottom: 0;
	right: 0;
	height: 40px;
	line-height: 40px !important;
	padding: 0 25px !important;
}
.form-group{
	position: relative;
}
.form-control{
	height: 40px;
}
.lock-screen {
	height: 100vh;
	width: 100%;
	display: flex;
    justify-content: center;
    align-items: center;        /* for single line flex container */
    align-content: center;      /* for multi-line flex container */

}

.bg-g1 {
	background: #7918f2;
	background: -webkit-linear-gradient(-45deg, #00F686, #0C00FF, #0BF6F6);
	background: -o-linear-gradient(-45deg, #00F686, #0C00FF, #0BF6F6);
	background: -moz-linear-gradient(-45deg, #00F686, #0C00FF, #0BF6F6);
	background: linear-gradient(-45deg, #00F686, #0C00FF, #0BF6F6);
}
</style>