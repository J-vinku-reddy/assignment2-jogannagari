# vinayaka reddy jogannagari
## miami

 >beautiful **beach** and different type of cuisines.Miami is a major center and leader in finance, commerce, culture, arts, and international trade.The metro area is by far the largest urban economy in Florida and the 12th largest in the United States, with a GDP of $344.9 billion as of 2017.In 2020, Miami was classified as a Beta + level global city by the GaWC.In 2019, Miami ranked seventh in the United States and 31st among global cities in business activity, human capital, information exchange, cultural experience, and political engagement.According to a 2018 UBS study of 77 world cities, the city was ranked as the third-richest in the world and the second-richest in the United States in purchasing power.**Miami is nicknamed the "Capital of Latin America" and is one of the largest majority-minority cities in the United States with over 72.7% of the population being of Hispanic and Latino descent.**

------

## Ordered list
1. Maryville
2. kansas city
    1. kansas airport
    2. terminal
    3. aeroplane
3. Miami
* backpack
    * good clothes
    * cosmotics
* camera
* food

**[LinktoAboutMe.md](AboutMe.md)**

-----

## Create food table
> To create a table with at least 4food/drinksthat you would recommend someone try.Include a short paragraph that introduces the table.

|mandatory     |fav1     |fav2     |fav3     |fav4     |
| :-----:      | :-----: | :-----: | :-----: | :-----: |
|food/drinks   |biryani  |pasta    |pizza    |pepsi    |
|location      |hyderabad|vizag    |delhi    |chennai  |
|amount        |50-40    |40-30    |30-20    |20-10    |

-----

## quotes by authors
>"whatever you are, but be good one".
Author: *valmiki* <br>
>"The purpose of our lives is to be happy".
Author: *parade* <br>

-----

## Code Fencing
>In the mathematical discipline of graph theory, a matching or independent edge set in an undirected graph is a set of edges without common vertices. Finding a matching in a bipartite graph can be treated as a network flow problem. source code <https://en.wikipedia.org/wiki/Matching_(graph_theory)#Definitions>

int n;
vector<vector<int>> adj;

vector<int> side(n, -1);
bool is_bipartite = true;
queue<int> q;
for (int st = 0; st < n; ++st) {
    if (side[st] == -1) {
        q.push(st);
        side[st] = 0;
        while (!q.empty()) {
            int v = q.front();
            q.pop();
            for (int u : adj[v]) {
                if (side[u] == -1) {
                    side[u] = side[v] ^ 1;
                    q.push(u);
                } else {
                    is_bipartite &= side[u] != side[v];
                }
            }
        }
    }
}

quick source code<https://cp-algorithms.com/graph/bipartite-check.html>
