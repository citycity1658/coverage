 /books:
   /{bookTitle}
     get:
       queryParameters:
         author:
           displayName: Author
           type: string
           description: An author's full name
           example: Mary Roach
           required: false
         publicationYear:
           displayName: Pub Year
           type: number
           description: The year released for the first time in the US
           example: 1984
           required: false
         rating:
           displayName: Rating
           type: number
           description: Average rating (1-5) submitted by users
           example: 3.14
           required: false
         isbn:
           displayName: ISBN
           type: string
           minLength: 10
           example: 0321736079?
      put:
        queryParameters:
          access_token:
            displayName: Access Token
            type: string
            description: Token giving you permission to make call
            required: true
