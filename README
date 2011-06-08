log4go, forked from http://log4go.googlecode.com/ to apply fixes and patches, and provide it as Git.


Installation
============

Run
	goinstall github.com/Kissaki/log4go


Usage
====

Add the following import:
	import l4g "github.com/Kissaki/log4go"

	// Formatted logging can be done at any of the logging levels (Finest, Fine, Debug, Trace, Info, Warning, Error, Critical)
	l4g.Trace("Received message: %s (%d)", msg, length)

	// Warnings, Errors, and Criticals provide an os.Error that you can use for a return
	return l4g.Error("Unable to open file: %s", err)

	// The wrapper functions can also behave like Sprint if the first argument isn't a string
	l4g.Debug(portno, clientid, client)

	// Use a closure so that if DEBUG isn't logged, it doesn't take any time
	l4g.Debug(func()string{ decodeRaw(raw) })

Log to a file:
	l4g.AddFilter("file", l4g.NewFileLogWriter("myapp.log", false))

Using example/example.xml as a base you can use a configuration file to set up logging:
	l4g.LoadConfiguration("logging.xml")

