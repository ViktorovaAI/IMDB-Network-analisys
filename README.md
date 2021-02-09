# IMDB-Network-analisys

This package contains the code for homework "Analysing Networks" prepared by A. Viktorova, D. Williams.


Is Kevin Bacon the center of the IMDB-Network?

Kevin Bacon is a very popular American actor, who starred in an unreasonably large
number of films. He himself once spoke out that everyone in Hollywood had either worked with him once, or worked with someone who worked with him. After that, they began to jokingly callit the center of the Universe, and in the local television show they came up with the concept of six degrees of Kevin Bacon.

To analyze the large IMDB datasets and make the volume manageable for our machines, we performed the following data cleansing activities:
❏ All not relevant attributes were removed.

❏ Only 'movie' and 'tvMovie' types were included, and other sypes, such as for example ‘videoGame’ and ‘tv series’, were excluded.

❏ Only categories ‘actor’ and ‘actress’ were included, while other categories (e.g. ‘director’, ‘producer’) were excluded from our dataset.

❏ Since the resulting network was still too large, we focused on the last decade: from the year 2010 to year 2020.

❏ Additionally we filtered for movies with IMDB ranking above 8.5 and number of voters more than 1000 (mean number of voters across the network is 960).


1. Which actor has smallest average distance to all others actors in IMDB (in the
large component)?

We calculated the closeness centrality for all the nodes in our largest connected component. As the result of the analysis the actor that has the smallest average distance in our IMDB subset appeared to be - Vijay Sethupathi, with the closeness centrality value of around 0.037.



2. Which actor has smallest maximum distance to all ...

We calculated eccentricity (he maximum distance from one node to all other nodes in the graph) for each node within the graph and then selected the minimum value to find the actor/actress who has the smallest distance to all other actors in IMDB. As the result of our analysis the actor that has the smallest maximum distance to all other actors and actresses appeared to be - Madhavan, with the eccentricity value - 2.
