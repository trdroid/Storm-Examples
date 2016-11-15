# Spout

A *spout* is the source of a *stream* in a *topology*.

![](_misc/Spout%20in%20a%20Topology.png)

### Data Sources

A *spout* normally reads data from an external data source by listening to

* Any message queues for incoming messages
* Any database for changes
* Any source of a data feed


### Emitting *tuples* or *streams*

A *spout* acts as a source of *tuples* or *streams* by reading data from a data source and emitting *tuples* or *streams* into the *topology*. 

### Receivers of *tuples* or *streams*

The nodes in a *topology* that a *spout* emits its *tuples* or *streams* to are known as *bolts*.
