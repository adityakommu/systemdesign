# systemdesign
Facebook contains billions of users and as a part of this system design exercise, we are going to introduce a news feed feature (pretend it does not exist). Below are some of the features and requirements of the system

1.  Each user when logged in should be displayed with a list of recent updates from the people / group / entity they follow or like
2. This must be timeline based (meaning the most recent updates first) - But feel free to choose your own logic on what basis you want to display. The algorithm is not important but be prepared to explain.
3. Users should be able to post media / text in their timeline.
4. The updates from the user to show up on their friends wall can have minimal latency. In other words, this does not have to be immediate.
5. User should be able to search for the post based on text in the post. This search should be limited to the friends / groups / entities that user follow.
6. Post should also be checked for "Explicit / Adult" content before posting successfully.
7. The news feed could potentially be loaded billion times in a day
8. You can expect each user to have, on average, 500 friends on the social network. You can treat the number of friends per user as a bell-shaped distribution, with some users who have very few friends, and some users who have a lot more than 500 friends.

Design only the core functionality of the feed. Scope limited to:

  - Load user's feeds (data model / strategy behind for faster loading)
  - Propagating status updates
  - Pipeline to check explicit content
  - Post status updates and search based on post text
  - System should be highly scalable / available and support millions of transactions per second
   - Let's design it using aws cloud 
