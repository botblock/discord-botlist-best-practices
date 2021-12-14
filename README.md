# Best Practices for Discord Bot Lists

---

*Bot lists must meet these minimum requirements to be considered a bot list.*

## Your bot list must:

1. use a custom domain name with a respectable, paid TLD (not `.tk`, `.ga` or any free domain provider from freenom or any services like that provide domains for free. For more info read [here](https://www.quora.com/Is-Freenom-a-fraudulent-company-I-registered-free-ccTLD-ga-and-tk-domain-names-and-within-a-few-2-3-days-all-of-the-domains-were-taken-away-and-marked-as-Fraud-without-any-explanation) and the notice to freenom [here](https://www.internetnews.me/wp-content/uploads/2015/09/serad-to-zuurbier-23jun15-en.pdf) (PDF)).
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
8. not be a copy of other's bot lists (such as vcodes, sank6, RDL, and others that are open sourced, including lists that are edited or modified from other's lists).

---

*Bot lists should meet these requirements to be a good bot list.*

## Your bot list should:

1. not display all bots on the homepage.
2. not be hosted on any free hosting provider.
3. be mobile friendly.
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
9. have a support (email and/or discord server) link on navbar or footer.
10. notify users beforehand when your tos or privacy pages are changing.

---

If anyone wants to change or add something, please make a pull request [here](https://github.com/botblock/discord-botlist-best-practices).

Inspired by [Discord Bot Best Practices](https://github.com/meew0/discord-bot-best-practices)
