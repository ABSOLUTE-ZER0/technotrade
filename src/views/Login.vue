<template>
	<b-container class="main" fluid>

		<b-row>
			<b-navbar class="nav-bar">
				<b-navbar-brand href="/">TechnoTrade</b-navbar-brand>
				<b-navbar-nav class="nav-items">
					<b-nav-item href="/register">Register</b-nav-item>
					<b-nav-item href="/about">About Us</b-nav-item>
					<b-nav-item href="/contact">Contact</b-nav-item>
				</b-navbar-nav>
			</b-navbar>
		</b-row>

		<b-row>
			<b-col offset-lg="8" lg="3">
				<h1 class="title">LOGIN</h1>
				<form class="main-form" action="#" method="post">
					<div class="form">
						<span class="fa fa-user" aria-hidden="true"></span>
						<div class="input-div">
							<input class="input" name="text1" id="text1" type="text" value="" placeholder="Username" required="">
						</div>
					</div>
					<div class="form">
						<span class="fa fa-lock" aria-hidden="true"></span>
						<div class="input-div">
							<input name="password" class="input" id="myInput" type="Password" placeholder="Password">
						</div>
					</div>
					<div class="input-div">
						<button type="submit" class="btn">Login</button>
					</div>
					<div class="logged-div">
						<b-form-checkbox class="loggedin" name="check-button" switch>Keep Logged In</b-form-checkbox>
						<a href="#" class="forgotpassword">forgot password?</a>
					</div>
					<div class="logged-div">
						<a href="/register" class="register">Create Account</a>
						<a href="#" class="help">NEED HELP?</a>
					</div>
				</form>

			</b-col>




		</b-row>
	</b-container>
</template>

<style scoped>
	.nav-items {
		margin-left: auto;
	}

	.title{
		font-family: fantasy;
		letter-spacing: 3px;
		margin-top: 40%;
	}

	.nav-bar {
		width: 100%;
	}

	.main {
		background-image: url("../assets/login.jpg");
		background-size: cover;
		height: 100vh;
		font-family: 'Mukta', sans-serif;
	}

	.form {
		display: flex;
		margin: 1em 0;
		background-color: rgba(128, 128, 128, 0.2);
		border-radius: 2em;
	}

	.form span {
		flex: 1;
		line-height: 3em;
		margin-top: 0.1em;
		text-align: right;
	}

	.main-form {
		margin-top: 20%;

	}

	.input {
		padding: 1em;
		background-color: transparent;
		border: 0;
		width: 100%;
	}

	.input:focus {
		outline: 0;
	}

	.input-div {
		flex: 4 50%;

	}

	.btn {
		background-color: rgb(252 99 107);
		width: 100%;
		border-radius: 2em;
		font-size: 1.2em;
		letter-spacing: 2px;
	}

	.logged-div {
		display: flex;
		margin-top: 1.5em;
		width: 100%;
		font-size: 0.9em;
	}

	.forgotpassword {
		color: rgb(83, 123, 255);
		margin-left: auto;
	}

	.register {
		text-transform: uppercase;
		font-weight: bold;
		color: rgb(83, 123, 255);

	}

	.help {
		text-transform: uppercase;
		font-weight: bold;
		margin-left: auto;
		color: rgb(83, 123, 255);

	}


  @media (max-width: 768px){
		.main{
					background-size: unset;
					font-size: 0.8em;

		}

		
	.title{
		margin-top: 25%;
	}

	}


</style>