<style>
/*----- Toggle Button -----*/
.toggle-nav {
	display:none;
}

/*----- Menu -----*/
.menu {
	width:100%;
	padding:10px 18px;
	box-shadow:0px 1px 1px rgba(0,0,0,0.15);
	border-radius:3px;
	background:#303030;
}

.menu ul {
	display:inline-block;
}

.menu li {
	margin:0px 50px 0px 0px;
	float:left;
	list-style:none;
	font-size:17px;
}

.menu li:last-child {
	margin-right:0px;
}

.menu a {
	text-shadow:0px 1px 0px rgba(0,0,0,0.5);
	color:#777;
	transition:color linear 0.15s;
}

.menu a:hover, .menu .current-item a {
	text-decoration:none;
	color:#66a992;
}

/*----- Search -----*/
.search-form {
	display:inline-block;
}

.search-form input {
	width:200px;
	height:30px;
	padding:0px 8px;
	float:left;
	border-radius:2px 0px 0px 2px;
	font-size:13px;
}

.search-form button {
	height:30px;
	padding:0px 7px;
	float:right;
	border-radius:0px 2px 2px 0px;
	background:#66a992;
	font-size:13px;
	font-weight:600;
	text-shadow:0px 1px 0px rgba(0,0,0,0.3);
	color:#fff;
}

/*----- Responsive -----*/

@media screen and (max-width: 970px) {
	.search-form input {
		width:120px;
	}
}

@media screen and (max-width: 860px) {
	.menu {
		position:relative;
		display:inline-block;
	}

	.menu ul.active {
		display:none;
	}

	.menu ul {
		width:100%;
		position:absolute;
		top:120%;
		left:0px;
		padding:10px 18px;
		box-shadow:0px 1px 1px rgba(0,0,0,0.15);
		border-radius:3px;
		background:#303030;
	}

	.menu ul:after {
		width:0px;
		height:0px;
		position:absolute;
		top:0%;
		left:22px;
		content:'';
		transform:translate(0%, -100%);
		border-left:7px solid transparent;
		border-right:7px solid transparent;
		border-bottom:7px solid #303030;
	}

	.menu li {
		margin:5px 0px 5px 0px;
		float:none;
		display:block;
	}

	.menu a {
		display:block;
	}

	.toggle-nav {
		padding:20px;
		display:inline-block;
		box-shadow:0px 1px 1px rgba(0,0,0,0.15);
		border-radius:3px;
		background:#303030;
		text-shadow:0px 1px 0px rgba(0,0,0,0.5);
		color:#777;
		font-size:20px;
		transition:color linear 0.15s;
	}

	.toggle-nav:hover {
		text-decoration:none;
		color:#66a992;
	}

	.search-form {
		margin:12px 0px 0px 20px;
		float:left;
	}

	.search-form input {
		box-shadow:-1px 1px 2px rgba(0,0,0,0.1);
	}
}
</style>

<nav class="menu">
	<ul class="active">
		<li class="current-item"><a href=".">Home</a></li>
		<li><a href=".">Explore</a></li>
		<li><a href=".">Profile</a></li>
		<li><a href=".">Buy License</a></li>
		<li><a href=".">Settings</a></li>
	</ul>

	<a class="toggle-nav" href=".">&#9776;</a>

	<form class="search-form">
		<input type="text">
		<button>Search</button>
	</form>
</nav>
