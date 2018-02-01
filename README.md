# GraphQL Android
The project has to applications:
<UL>
<LI>First is ApolloGraphQLExample which uses apollo-android to auto generate the necessary JAVA models for graphQL queries.</LI>
<LI>Second is GraphQL which uses retrofit by just posting up raw queries with appropriate headers on the URL and getting results.</LI>
</UL>
<br>
The first method is most recommended because it auto generates the code for models according to your queries. The advantage is that it decouples the graphql queries from the code which makes easier to code.<br>
<b>Query used</b><br>
<pre>
query {
  repository(owner:"jakewharton", name:"butterknife") {
    name
    description
    forkCount
    url
  }
}
</pre>
<br>
<pre>
query {
  repository(owner:"amanjeetsingh150", name:"ubercaranimation") {
    name
    description
    forkCount
    url
  }
}
</pre>
The result of the above query is shown below:

<b>Screenshots:</b>
<br><br>
<img src="graphql.gif"/>&nbsp; &nbsp;<img src="apollo.gif"/>
