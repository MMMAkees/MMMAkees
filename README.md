## Hi there 👋
name: Latest blog post workflow
on: 
    schedule:
        - cron: '0 * * * *'
jobs: 
    update-readme-with-blog: 
        name: Update this repo's README with latest blog posts
        runs-on: ubuntu-latest
        steps: 
            - uses: actions/checkout@v2
            - uses: gautamkrishnar/blog-post-workflow@master
              with: 
                max_post_count: "4"
                feed_list: "https://dev.to/feed/mmmakees"
<!--
**MMMAkees/MMMAkees** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
