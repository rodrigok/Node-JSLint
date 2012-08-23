[![build status](https://secure.travis-ci.org/rodrigok/Node-JSLint.png)](http://travis-ci.org/rodrigok/Node-JSLint)
<h1>Instalation</h1>
<p>
	This script don't require instalation, you only need download this files and execute as below.
	If you has the NPM instaled you can install this script via NPM:
	<ul>
		<li>
			Into your project:
			<pre>npm install JSLintCli</pre>
		</li>
		<li>
			As Global (Recomended):
			<pre>sudo npm install JSLintCli -g</pre>
			If you install as Global you need execute this script as SuperUser on the first time to download and install the core
		</li>
	</ul>
</p>

<h1>Usage</h1>
<p>
	There are 2 ways to execute this script:
	<ul>
		<li>
			Using node executable:
			<pre>node JSLint</pre>
		</li>
		<li>
			Or using JSLint as executable:
			<pre>./JSLint</pre>
		</li>
	</ul>
</p>
<p>
	You can pass to this script one of this file formats:
	<ul>
		<li>
			One file:
			<pre>node JSLint tests/test1.js</pre>
		</li>
		<li>
			Multiple files:
			<pre>node JSLint tests/test1.js tests/test2.js tests/test3.js</pre>
		</li>
		<li>
			A search with wildcard:
			<pre>node JSLint tests/*.js</pre>
		</li>
	</ul>
</p>
<p>
	This script accept one option parameter (--list). With this parameter the script don't show the list of errors, only show a list of files that was passed and your status after the JSLint validation:
	<pre>node JSLint --list tests/*.js</pre>
	The return will be like this:
<pre>
>tests/test1.js - 3 problem(s) found
>tests/test2.js - No problems found
>tests/test3.js - No problems found
>tests/test4.js - 2 problem(s) found</pre>
</p>

<h1>First Time</h1>
<p>
	When you execute this script the first time, this script will download the JSLint core from https://raw.github.com/douglascrockford/JSLint/master/jslint.js.
	After download, the script will execute normally.
<p>