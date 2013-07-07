# README

This is a simple project designed to estimate how long it will take to
refill the batteries in your Tesla Model S. Really, it should work for
pretty much any EV.

# Current Status

This is a "stake in the ground" implementation, so don't trust it. I
am trying to make sure the formulas I'm using are correct and actually
are based in fact.

The operating assumption is that Ohm's "power" formula:

W = V x I

is applicable to how we charge our EV batteries. So, for example,
if I charge my batteries on a 240V / 40A circuit, I should get 9.6 kW.

Assuming that I need 50kWh to get to my next destination, simple
division shows that I will have to wait at that charging station
for 5.21 hours. That's probably a best case scenario.

I don't factor resistance or ramp up/down into my calculations.

# What's Next

Right now, it's barely acceptable on mobile devices. It would be nice
to make it easier to use. Maybe using jQuery Touch or something.

There are no graphics or other cool things in this site. Anything
would be better than nothing!

Calculations are not "live" everywhere, so the actual results don't
update as you change the inputs. That's why the "calculate" button
is there. No reason that should be true.

# How It's Implemented

This is a trivial site implemented using [Middleman](https://github.com/middleman/middleman),
HTML5, [Twitter Bootstrap](http://twitter.github.io/bootstrap/index.html), jQuery (http://jquery.com),
and Coffeescript (http://coffeescript.org).

As a side benefit, it uses both [Haml](http://haml.info) and [Sass](http://sass-lang.com) to create
loveable markup.

# How to Contribute

This was a quick stab at implementing. If you want to help make it nicer, fork the project,
polish it up or fix a problem, and submit a pull request. If you don't know how to do that,
well ... you can report a bug using GitHub issues.