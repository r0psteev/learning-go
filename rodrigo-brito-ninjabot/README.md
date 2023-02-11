# Project description.

A fast trading bot.
At the time of writing is supports Binance.


## go embed

https://github.com/rodrigo-brito/ninjabot/blob/348caa02a90e1e16ec25e0a588bd67744903baf4/plot/chart.go#L25-L28

In this line, @rodrigo-brito uses the go embed ability to embed a static html directory into
the final bot binary that will be created.

I think such ability is really intresting in the sense that it could also be applied to build
artifacts from higher frameworks like react/vue, and have them shipped with a single binary.
