Users
{
  id: autoincrement,
  first_name: string,
  last_name: string,
  email: string,
  username: string,
  password: string,
  profile:
      {
        about: text,
        photo: image,
        friend_total: integer,
      }
  friends: array[user_id]
  photos: array[photo_id]
  posts: array[post_id]
  comments: array[comment_id]
  reaction: array[reaction_id]
}
Photos
{
  id: autoincrement,
  content: img,
  user_id: integer,
  comment: array[comment_id]
  reaction: array[reaction_id]
}
Posts
{
  id: autoincrement,
  content: text,
  user_id: integer,
  comment: array[comment_id],
  reaction: array[reaction_id]
}
Comments
{
  id: autoincrement,
  content: text,
  user_id: integer,
  comment: array[comment_id],
  reaction; array[reaction_id]
}
Reaction
{
  id: autoincrement,
  content: image,
  user_id: integer
  comment: array[comment_id]
}

* username: String
    * Must contain only word characters
* password: String
    * Must be at least 8 characters
* email: String
    * Must containt '@'
* photo: image
    * Must be in jpeg, gif, or png format,
    * Must not exceed x MB


* Alg to determine "often interaction" between users.
