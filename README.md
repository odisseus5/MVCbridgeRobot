# MVCbridgeRobot

MVC for free bridge robot

The issue is interesting for the gaming community:

https://github.com/lorserker/ben
https://bridgewinners.com/article/view/free-and-open-source-bridge-ai-engine-released/

Robots are playing OK, but still people play better for the time being.

My point is to apply Model-View-Controller (MVC) design pattern to the specific bridge case.

https://www.bridgebase.com/v3/

developed .lin messaging format in which a hand is described by at most 13 characters

A,K,Q,J,T,9,8,7,6,5,4,3,2

One can order suits (and bids)

C,D,H,S,N,x,xx

Introduce flags (visible, vulnerable, on lead, etc), there is no point to go into detail, but it is clear, that messaging is compact.

View is whatever you prefer - local executable, web service…

Model - database, history, analytics.

Controller is the most interesting part:

Bridge rules
Bidding systems, standard agreements, etc

AI to choose next bid or next card to put on the table.

Remark

I think that Bidding systems should be part of the Controller taking into account practical applications:

Suppose you are an user having to play with robot and you vaguely know that you are playing SAYC, Stayman, transfers to majors, and everything std.

Robot messages: 

your system is fine, p,

and plays your system


