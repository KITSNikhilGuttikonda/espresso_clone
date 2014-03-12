##### This is a clone of https://code.google.com/p/android-test-kit/source/checkout as of 2014-03-12

###

This is Google's Espresso 1.1 with a boolean "exists()" added to the ViewInteraction class.
This allows one to write code like:

if(onView(withText("click OK to Continue")).exists()){
	doSomething();
} else {
	doSomethingElse();
}

Please be aware that Espresso does not contain such funtionality by design, according one of it's Authors at http://stackoverflow.com/questions/20807131/espresso-return-boolean-if-view-exists

To compile:

- Ubuntu 12.04 LTS
- sun java version "1.7.0_51"
- android sdk 19 (kitkat)
- mvn install

by the way, it fails compiling the tests, just like the original Espresso code does, but since I need just ./espresso/lib/target/espresso-1.1-bundled.jar
, I am happy with the results


Marcos Diez ( marcos AT unitron DOT com DOT br)