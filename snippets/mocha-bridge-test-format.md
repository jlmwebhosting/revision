//: @ignore:
//: @end-ignore


//: @bridge:

describe( "<module>", ( ) => {

	let bridgeURL = `file://${ path.resolve( __dirname, "bridge.html" ) }`;

} );

//: @end-bridge

describe( "`<test>`", ( ) => {
	it( "<message>", ( ) => {

		let result = browser.url( bridgeURL ).execute(

			function( ){
				return <test>;
			}

		).value;

		assert.equal( result, <expected> );

	} );
} );
