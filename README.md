- install json server globally
  npm i json-server -g
- start json-server
  json-server --watch data/db.json --port 3500

- Le fait d'utiliser le `providesTags: ['Todos']` et `invalidatesTags: ['Todos']` permet le rerender.
    A query can have its cached data provide tags. Doing so determines which 'tag' is attached to the cached data returned by the query.
    A mutation can invalidate specific cached data based on the tags. Doing so determines which cached data will be either refetched or removed from the cache.