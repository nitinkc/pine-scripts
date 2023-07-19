
```
plot(rsi, title="equity", color=color.red, linewidth=2, style=plot.style_linebr)

plotshape(crossoverMid, style=shape.cross, size = size.tiny, color = color.aqua, location = location.belowbar)
plotshape(crossunderMid, style=shape.diamond, size = size.tiny, color = color.aqua, location = location.belowbar)

plotchar(goldenCrossover, "Go Long",  "▲", location.abovebar, color.lime, size = size.normal)
```

Plot the shape

```
plotshape(buyEntry, title="Buy", text="Buy", location=location.absolute, style=shape.labelup, size=size.tiny, color=color.green, textcolor=color.white, transp=0)


plotshape(sellEntry, title="Sell", text="Sell", location=location.absolute, style=shape.labeldown, size=size.tiny, color=color.red, textcolor=color.white, transp=0)
```

Change the colour of the plot

```
c = close >= open ? color.lime : color.red
plot(close, color = c)
```
