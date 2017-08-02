$ONCEdescribe( "<module>", ( ) => {

	let bridgeURL = `file://${ path.resolve( __dirname, "bridge.html" ) }`;

$EACHdescribe( `"$row"`, ( ) => {
		it( "<message>", ( ) => {

			let result = browser.url( bridgeURL ).execute(

				function( ){
					return $row;
				}

			).value;

			assert.equal( result, <expected> );

		} );
} );

$ONCE} );
