//: @ignore:
//: @end-ignore


//: @bridge:

describe( "<module>", ( ) => {

} );

//: @end-bridge

describe( `"<test>"`, ( ) => {
	it( "<message>", ( ) => {

		let result = browser.url( bridgeURL ).execute(

			function( ){
				return <test>;
			}

		).value;

		assert.equal( result, <expected> );

	} );
} );
