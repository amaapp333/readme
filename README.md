# readme


wpcom-proxy-request
Proxied cookie-authenticated REST-API and WP-API requests to WordPress.com

You likely want to use the high-level APIs in wpcom.js instead of using this module directly.

This module offers access to the WordPress.com REST-API and WP-API via a proxying <iframe> pointing to a special URL that proxies API requests on the host page's behalf.

It is intended to be used in the browser (client-side) via a bundler like browserify or webpack.

Installation
Install wpcom-proxy-request using npm:

npm install wpcom-proxy-request
Example
// Import wpcom-proxy-request handler
import proxy from 'wpcom-proxy-request';

proxy( { path: '/me' }, function ( err, body, headers ) {
	if ( err ) {
		throw err;
	}

	const div = document.createElement( 'div' );
	div.innerHTML = 'Your WordPress.com "username" is: <b>@' + res.username + '</b>';
	document.body.appendChild( div );
} );
Running tests
Compile and watch client-test application

make watch-test-app
Run server

make run-test-app
Open a tab pointing to http://calypso.localhost:3001/

License
MIT – Copyright Automattic 2014

Keywords
browserwpcomwordpressrestapicookie
Install
npm i wpcom-proxy-request

Repository
github.com/Automattic/wp-calypso

Homepage
github.com/Automattic/wp-calypso

Weekly Downloads
270

Version
6.0.0

License
MIT

Unpacked Size
36.3 kB

Total Files
7

Issues
4098

Pull Requests
453

Last publish
2 years ago

Collaborators
