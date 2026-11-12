# HostelMate MCP server

Ask Claude or ChatGPT about your hostel: who checks in today, who still owes money, what you made last month.
The HostelMate MCP server connects the [HostelMate hostel management software](https://hostelmate.co/) to AI
assistants over the Model Context Protocol. It is read-only and signs in with your own HostelMate login.

- **Server address:** `https://mcp.hostelmate.co/mcp` (Streamable HTTP, OAuth sign-in)
- **Claude:** listed in Claude's connector directory: [HostelMate in Claude](https://claude.ai/directory/hostelmate)
- **Official MCP Registry:** `io.github.hostelmate/hostelmate`
- **Product page:** [hostelmate.co/app/mcp](https://hostelmate.co/app/mcp)
- **Setup guide:** [docs.hostelmate.co/connect-claude-chatgpt](https://docs.hostelmate.co/connect-claude-chatgpt)

## What you can ask

| Area | Example questions |
|---|---|
| Front desk | Who checks in today? Who arrives and who leaves today? |
| Bookings | Show me this week's Booking.com bookings. Is anything double-booked this weekend? |
| Payments and revenue | How much has Maria paid? What did we make last month? Daily revenue since 1 September. |
| Properties | List my properties. |

Revenue answers are for managers, and they aren't part of the [Lite plan](https://hostelmate.co/pricing). If you run
more than one hostel, name the property in your question.

## Connect it

**Claude** (web, desktop, iPhone and Android, every plan):

1. Open [HostelMate in Claude's directory](https://claude.ai/directory/hostelmate) and click **Connect**.
2. Sign in with your HostelMate email and password, then click **Sign in** and **Allow**.

Or in Claude: **Connectors** → **Add custom connector** → paste `https://mcp.hostelmate.co/mcp` → **Add** → **Connect**.
On Team and Enterprise plans, an owner switches connectors on for the organisation first.

**ChatGPT** (Plus, Pro, Business and Enterprise, in the browser):

1. **Settings** → **Apps** → **Advanced** → turn on **Developer mode**.
2. Create an app with the address `https://mcp.hostelmate.co/mcp` and choose **OAuth**.
3. Sign in with your HostelMate email and password.

**Other MCP clients:** add a remote server with the address above; the client opens HostelMate's sign-in page.

## What the assistant can and can't see

- **Read-only.** It can look things up, but it can't create, change or cancel a booking, a payment or anything else.
- **Your own permissions.** It signs in as you, so it sees what you see in HostelMate.
- **Guest details stay out.** Guest phone numbers, emails, passports and card details are never shared with the assistant.
- **Your password stays with HostelMate.** The assistant never sees it.
- **20 days at a time.** You stay connected for 20 days, then sign in again. Remove HostelMate in your connector
  settings to disconnect sooner.

## About HostelMate

[HostelMate](https://hostelmate.co/) is hostel management software built around the bed: a
[property management system](https://hostelmate.co/pages/about/hostel-management-system), a
[channel manager](https://hostelmate.co/features/channel-manager) and a commission-free [booking engine](https://hostelmate.co/features/hostel-booking-engine-calendar) in one product.

Questions: contact@hostelmate.co
