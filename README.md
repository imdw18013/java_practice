# java_practice
# COMP2112-Lab 6
## ES6+ features:
## *1).map function*: This function creates a new array with the results of calling a new function for each array element. Map is a collection of elemetes where each element is stored as key and value. It returns the key, value pair in the same order as inserted. We have used map function in our twitter page where we fetched the values and stored them into array to return the same value.
# [More details about .map functions!] https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
``` javascript  "function render() {
  main.innerHTML = tweets.map(tweet =>`
        <aside>
         <div>
            <img class="avatar" src="${tweet.avatar}">
         </div>
         <div class="formatted-tweet">
            <h6><a href="https://twitter.com/${tweet.username}">${tweet.name}</a> <span class="username">@${tweet.username}</span></h6>
            <p>${tweet.tweet}</p>
            <div class="imgGifPoll">
            </div>
            <div>
                <section>
                    <div id="reactions" class="btn-group mr-2">
                        <button
                            type="button"
                            class="btn btn-secondary mdi mdi-message-outline"
                            aria-label="reply"
                        ></button>
                        <button
                            type="button"
                            class="btn btn-secondary mdi mdi-twitter-retweet"
                            aria-label="retweet"
                        ></button>
                        <button
                            type="button"
                            class="btn btn-secondary mdi mdi-heart-outline"
                            aria-label="like"
                            style=""
                        ></button>
                        <button
                            type="button"
                            class="btn btn-secondary mdi mdi-upload"
                            aria-label="share"
                        ></button>
                    </div>
                </section>
            </div>
        </div>
        </aside>
          `).join('');
}" ```
