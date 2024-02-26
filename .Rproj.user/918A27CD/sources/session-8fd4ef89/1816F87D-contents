library("here")
library("sf")
library("rmapshaper")
library("svglite")

#Geodaten einlesen
bl <- st_read(here("daten","nuts250_12-31.utm32s.shape", "nuts250_1231", "NUTS250_N1.shp"))

by <- bl[which(bl$NUTS_NAME=="Bayern"),]
by_mss <-ms_simplify(by, keep=0.01)

plot(st_geometry(by_mss))
#IF gelb: #f9b000
#IF blau: #173853

st_crs(by)

