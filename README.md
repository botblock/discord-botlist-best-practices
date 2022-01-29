# Best Practices for Discord Bot Lists

---

*Bot lists must meet these minimum requirements to be considered a bot list.*

## Your bot list must:

1. use a custom domain name with a respectable, paid TLD.
2. not be a `[xyz].glitch.me`, `[xyz].repl.co` or any free (sub)domain with free hosting provider.
   - Glitch, Repl, or any other free host is acceptable if:
      - Uptime is immaculate
      - A custom domain name is used (whilst still following point `1`)
3. be fully functioning.
   - No broken links/buttons.
4. have consistent uptime.
   - Minor downtime for maintenance or fixing issues is fine
5. have bot listing requirements (such as no NSFW outside NSFW channels, respect rate-limits, don't respond to other bots, etc.)
6. blur NSFW profile pictures.
7. have a ToS and Privacy page.
8. make it clear that you are not affiliated with Discord.
9. have support for slash bots (like letting prefix to be not set, let users know whether this bot is slash command only or slash + bot, or bot only, etc.)
10. not serve broken images, maybe let the broken images get replaced with custom image.

---

*Bot lists should meet these requirements to be a good bot list.*

## Your bot list should:

1. not display all bots on the homepage, the footer should be reachable without loading more and more bots.
2. not be hosted on any free hosting provider.
3. be mobile and tablet friendly.
4. not be paid access only.
5. have an API with good documentation.
   - API should support `GET`ting bot information
      - Sends a JSON body for the response data
   - API should support `POST`ing bot stats
      - Server/guild count
      - Shard support
      - Uses an Authorization header
      - Accepts a JSON body format for data
6. respond with correct status codes.
   - All pages that load correctly should respond with a 2xx status code
   - Not found (404) pages should respond with a 404 status code
   - Any API should also send correct status codes
7. not overuse ads. Ads are okay, but shouldn't influence the browsing experience in a negative way.
8. have API (and the frontend if possible) ratelimits. (60 requests per minute recommended)
9. have a way for users to contact the folks operating the site (email, Discord, etc.).
10. notify users beforehand when your TOS or privacy policy is changing.
11. not be a copy of other's bot lists (open sourced lists, including lists that are edited or modified from other's lists).
12. have a better way of handling errors, instead of showing console errors, show a custom 500 status code page.
13. load fast enough, and use not a lot of time and/or internet data to load your site for the first time.
14. have a caching system in place.
15. not have a custom keybind to stop browser dev tools from loading.
16. save users from getting xss attacks.
17. sanitize bot's long description.
18. allow custom css.
19. store markdown, render it as html on user's request.
20. be usable on safari web browsers (both on iOS and Mac), Apple breaks your site on safari most of time, please check it out (maybe via browser stack).
21. not have NSFW ads, whilst following rule no. 7
22. not share user sensitive data without user's consent.
23. have a cookie consent on new visit.
24. save user from malicious links
25. should not freeze user's browser and/or operating system.

---

If anyone wants to change or add something, please [make a pull request](https://github.com/botblock/discord-botlist-best-practices).

Inspired by [Discord Bot Best Practices](https://github.com/meew0/discord-bot-best-practices)
