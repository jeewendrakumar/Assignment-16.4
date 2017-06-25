# Assignment-16.4

{"query":"mutation AddBookMutation($input_0:AddBookInput!) {\n  addBook(input:$input_0) {\n    clientMutationId,\n    ...F4\n  }\n}\nfragment F0 on BookStore {\n  id\n}\nfragment F1 on BookStore {\n  id,\n  ...F0\n}\nfragment F2 on BookStore {\n  id,\n  ...F1\n}\nfragment F3 on BookStore {\n  id,\n  ...F2,\n  ...F0\n}\nfragment F4 on AddBookPayload {\n  bookEdge {\n    cursor,\n    __typename,\n    node {\n      id,\n      title,\n      author\n    }\n  },\n  bookStore {\n    id,\n    ...F3\n  }\n}","variables":{"input_0":{"title":"TESTRING","author":"TESTING","clientMutationId":"0"}}}
