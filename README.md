# Best Practices for Discord Bot Lists

---

*Bot lists must meet these minimum requirements to be considered a bot list.*

## Your bot list must:

1. use a custom domain name with a respectable, paid TLD.
2. not be a `[xyz].glitch.me` domain.
   - Glitch is acceptable if:
      - Uptime is immaculate
      - A custom domain name is used (whilst still following point `1`)
3. be fully functioning.
   - No broken links/buttons.
4. have consistent uptime.
   - Minor downtime for maintenance or fixing issues is fine
5. Have minimum bot requirements (such as but not limited to, no NSFW outside NSFW channels, respect ratelimites, etc.)

---

*Bot lists should meet these requirements to be a good bot list.*

## Your bot list should:

1. not display all bots on the homepage.
2. not be hosted on Glitch or any other free host
3. be mobile responsive.
4. have an API with good documentation.
   - API should support `GET`ting bot information
      - Sends a JSON body for the response data
   - API should support `POST`ing bot stats
      - Server/guild count
      - Shard support
      - Uses an Authorization header
      - Accepts a JSON body format for data
5. respond with correct status codes.
   - All pages that load correctly should respond with a 2xx status code
   - Not found (404) pages should respond with a 404 status code
   - Any API should also send correct status codes

---

If anyone wants to change or add something, please make a pull request.

Inspired by [Discord Bot Best Practices](https://github.com/meew0/discord-bot-best-practices)
