# GO - Angular 2 QuickStart Final

See the angular site for the quickstart for angular 2.
This project source starts at the endpoint of the quickstart as of 6/21/2016 and the source was pulled from the plunk.zip file
available at that time.

To start a the simplest possible go integration for the first step of this same quickstart check out
[GO - Angular 2 QuickStart](https://github.com/andgrit/goangularquickstart)


# Go server integraion

This main program will do the trick.
I chose github.com/gorilla/mux for the mux instead of the standard library because it is great and I use it for all projects.
Compile and run from the goservrer directory, 
notice the ".." in `r.PathPrefix("/").Handler(http.FileServer(http.Dir("../angular")))`

    git clone ...
    cd PROJECT/angular
    npm install
    npm install -g tsc
    npm run tsc

At this point you could run as described in the original turorial.  
But lets start things up using go

    cd ../goserver
    go get -v
    go build
    ./goserver

