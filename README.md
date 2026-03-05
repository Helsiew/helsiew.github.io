<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Helena Siew — Marketing Portfolio</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.2.0/umd/react.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.2.0/umd/react-dom.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/7.23.2/babel.min.js"></script>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body { background: #f7f7f7; color: #0a0a0a; font-family: Georgia, 'Times New Roman', serif; font-size: 16px; line-height: 1.6; overflow-x: hidden; }
</style>
</head>
<body>
<div id="root"></div>
<script type="text/babel">
const data = {
  hero: {
    eyebrow: "Brand & Marketing Manager · SG / MY",
    headline: "A jack of all trades is better than a master of one.",
    bio: "A versatile marketing strategist with a passion for building brands that resonate. With experience spanning Government, BSFI, lifestyle, tech, and DTC, I craft marketing strategies that blend creative storytelling with data-driven precision to deliver measurable impact.",
    stats: [
      { val: "84%", label: "Uplift in restaurant covers within 7 days" },
      { val: "76.8M", label: "Impressions on a single festive campaign" },
      { val: "5×", label: "Industry award wins across SG & MY markets" },
    ],
  },
  expertise: [
    { num: "01", title: "Revenue Growth & Customer Acquisition" },
    { num: "02", title: "Brand Strategy & Market Positioning" },
    { num: "03", title: "CRM, Loyalty & Retention" },
    { num: "04", title: "Performance Marketing & Optimisation" },
  ],
  campaigns: [
    {
      num: "01", employer: "Harry's International",
      title: "Marketing, Brand Repositioning & New Menu Launches",
      desc: "Led the go-to-market strategy for new menu offerings — including Lunch offerings, Weekend & Daily Menu launches, and Christmas Specials — as part of a wider brand repositioning effort. Deployed a 1-for-1 promotional mechanic to overcome brand blind spots and drive trial visits, using performance digital campaigns across paid social, email, and search to generate footfall and amplify the new menu offerings' visibility.",
      metrics: [
        { val: "84%", label: "Increase in covers within 7 days" },
        { val: "+15%", label: "Uplift in total receipts" },
        { val: "200%", label: "YoY website traffic growth" },
      ],
      links: [
        { label: "Instagram 1", url: "https://www.instagram.com/reel/DOxr_RfDJ1z/" },
        { label: "Instagram 2", url: "https://www.instagram.com/reel/DQTYu6aDVAD/" },
        { label: "Instagram 3", url: "https://www.instagram.com/reel/DSq6oHOjb-a/" },
        { label: "CNY 2026 Post", url: "https://www.instagram.com/p/DTzzm9ok-3z/?img_index=4" },
        { label: "CNY 2026 Reel", url: "https://www.instagram.com/reel/DUFkd9Cku-g/" },
      ],
      tags: ["Email Marketing", "Paid Ads", "Digital Campaigns", "Brand Strategy"],
    },
    {
      num: "02", employer: "Harry's International",
      title: "Loyalty Programme Refresh — Win a Business Class Trip to Koh Samui",
      desc: "Redesigned the loyalty programme to re-engage lapsed members and drive new sign-ups through a high-value contest mechanic: a business class trip to Koh Samui co-sponsored by a travel partner and resort. Managed end-to-end execution: Web UI/UX, CRM flows, email, paid amplification, and sponsorship negotiation.",
      metrics: [
        { val: "82%", label: "Revenue achieved vs KPI" },
        { val: "~90%", label: "New sign-up target attained" },
        { val: "2.4×", label: "Average return customer rate" },
      ],
      links: [
        { label: "Instagram 1", url: "https://www.instagram.com/reel/DRBPNOrAu_s/" },
        { label: "Instagram 2", url: "https://www.instagram.com/reel/DQrBM9Kj_Vp/" },
        { label: "Instagram 3", url: "https://www.instagram.com/reel/DQG37P0CHoJ/" },
        { label: "Instagram 4", url: "https://www.instagram.com/reel/DP3cTCzggtm/" },
      ],
      tags: ["CRM & Loyalty", "Email Marketing", "Web UI/UX", "Paid Ads", "Sponsorships"],
    },
    {
      num: "03", employer: "Harry's International",
      title: "Eat.Play.Race — F1 Season Brand Activation with Razer & 99bends",
      desc: "Secured a tri-party partnership with Razer and 99bends to install a racing simulator experience across Harry's outlets during Singapore's F1 season. Recognised by the Singapore Tourism Board as a participating local brand, the campaign extended Harry's relevance beyond F&B into lifestyle and motorsport culture.",
      impact: "⭐  STB-Recognised F1 Local Brand Participant",
      tags: ["Brand Partnerships", "Sponsorships", "Experiential", "Digital Campaigns"],
    },
    {
      num: "04", employer: "Publicis · Client: Singapore Police Force",
      title: "Anti-Scam Awareness Campaign 2025",
      desc: "Architected the full-year content strategy for SPF's 2025 anti-scam initiative across multiple scam verticals. Orchestrated a multi-publisher and creator ecosystem to deliver education-first content at scale, translating complex behavioural messaging into platform-native formats that earned genuine public engagement and industry recognition.",
      impact: "🥇  GOLD — MEA Excellence in Content Marketing 2025",
      links: [{ label: "Watch Campaign", url: "https://www.youtube.com/watch?v=TvyEbtZh_0w" }],
      tags: ["Content Strategy", "Creator Partnerships", "Public Education", "Government"],
    },
    {
      num: "05", employer: "Publicis · Client: SCDF",
      title: 'SCDF "What\'s Your Emergency?" (2023–2024)',
      desc: "Strategised a two-year content campaign with three measurable public behaviour objectives: reducing misuse of 995, building awareness of non-emergency alternatives, and gaining public acceptance of SCDF's non-conveyance policy. Used platform-native storytelling on TikTok and social to make compliance messaging culturally resonant, earning 3 industry awards across 2 years.",
      metrics: [
        { val: "🏆", label: "TikTok Best Branding Campaign 2024" },
        { val: "🥈", label: "MEA Brand Awareness Silver 2024" },
        { val: "🥉", label: "Markies Gov/Non-Profit Bronze 2023" },
      ],
      links: [{ label: "Watch Campaign", url: "https://www.youtube.com/watch?v=GHIui58LRzw" }],
      tags: ["Content Strategy", "Behaviour Change", "TikTok", "Government"],
    },
    {
      num: "06", employer: "Publicis · Client: Building & Construction Authority",
      title: "Reframing the Industry for Young Talent",
      desc: "Countered entrenched 'blue collar' perceptions of Singapore's built environment sector through documentary-style content. Featured high-tech projects (Sensoryscape, Deep Tunnel Sewerage System Phase 2) and spotlighted women in construction engineering, delivering across YouTube, Facebook, Instagram, and TikTok to reach a younger workforce audience.",
      impact: "📱  Multi-platform content series across YouTube, Facebook, Instagram & TikTok",
      links: [
        { label: "YouTube", url: "https://youtube.com/watch?v=gTT61QRZfGA" },
        { label: "Facebook", url: "https://www.facebook.com/ourgrandfatherstory/videos/332091059953617/" },
        { label: "Instagram", url: "https://www.instagram.com/reels/C9MD6gVyg6o/" },
        { label: "TikTok", url: "https://www.tiktok.com/@sgag_sg/video/7332040142045056258" },
      ],
      tags: ["Content Strategy", "Employer Branding", "Video", "Social Media"],
    },
    {
      num: "07", employer: "Publicis · Client: Land Transport Authority",
      title: "People Behind the Tracks",
      desc: "Created a human-led documentary content series spotlighting the workforce keeping Singapore's public transport network running, in partnership with SMRT, SBSTransit, and other operators. Turned institutional messaging into personal stories that built public appreciation for the industry and strengthened LTA's employer brand positioning.",
      impact: "🎬  3-part video series in partnership with SMRT, SBS Transit & transport operators",
      links: [
        { label: "Episode 1", url: "https://www.youtube.com/watch?v=wFBgEr3yd_0" },
        { label: "Episode 2", url: "https://www.youtube.com/watch?v=hBWetPOB2oQ" },
        { label: "Episode 3", url: "https://www.youtube.com/watch?v=byZh0D0THOI" },
      ],
      tags: ["Content Strategy", "Employer Branding", "Documentary Series", "Government"],
    },
    {
      num: "08", employer: "Jirnexu / RinggitPlus",
      title: "Malaysian Financial Literacy Survey 2022",
      desc: "Owned the annual national financial research study from strategy through go-to-market, including sponsorship development and stakeholder management. The survey established RinggitPlus as a credible authority on Malaysian personal finance behaviour, generating media coverage and brand visibility across the financial services landscape.",
      links: [
        { label: "View Report", url: "https://ringgitplus.com/en/ringgitplus-malaysian-financial-literacy-survey-2022/" },
      ],
      tags: ["Brand Planning", "Social Media Strategy", "Research", "Go-to-Market", "Stakeholder Management", "Financial Services"],
    },
    {
      num: "09", employer: "Reprise · Client: UEM Sunrise",
      title: "The Happy Chase — Property Gameshow Campaign",
      desc: "Designed a gamified campaign strategy for Malaysian property developer UEM Sunrise, addressing post-pandemic purchase hesitancy with an interactive gameshow format and a low-barrier RM1 booking fee mechanic. The campaign turned brand entertainment into a tangible sales pipeline, generating leads at nearly double the original target.",
      metrics: [
        { val: "747", label: "Leads generated vs 400 target" },
        { val: "27M", label: "Total impressions" },
        { val: "696K", label: "Video views" },
        { val: "49K", label: "Engagements" },
      ],
      links: [
        { label: "The Edge", url: "https://theedgemalaysia.com/article/uem-sunrise-launches-happy-chase-gameshow-0" },
        { label: "Malaysian Reserve", url: "https://themalaysianreserve.com/2020/08/18/uem-sunrise-launches-the-happy-chase-gameshow/" },
      ],
      tags: ["Campaign Strategy", "Gamification", "Lead Generation", "Social Media"],
    },
    {
      num: "10", employer: "Ogilvy · Client: CIMB",
      title: "CIMB Chinese New Year — Cinematic & Interactive Festive Campaign 2019",
      desc: "Executed a multi-format festive campaign anchored by a cinematic Yee Sang origin film and an interactive mobile game, transforming a traditional CNY banking campaign into a platform that audiences chose to spend time with. Exceeded every KPI set by the client, earned a shortlist at the APPIES Awards, and was rated a top CNY ad of 2019 by Campaign Asia.",
      metrics: [
        { val: "76.8M", label: "Total impressions" },
        { val: "14.2M", label: "Total engagements" },
        { val: "11.3M", label: "Video views" },
        { val: "167K", label: "Mobile game plays" },
        { val: "31.6K", label: "Game visitors" },
        { val: "13.5K", label: "Registered players" },
      ],
      links: [
        { label: "Watch Campaign", url: "https://aws2.campaignasia.com/video/yee-sang-gets-a-cinematic-origin-story/449689" },
      ],
      tags: ["Campaign Execution", "Gamification", "Video", "Financial Services"],
    },
  ],
  additional: [
    { title: "MDDI Anti-Cyberbullying", employer: "Publicis", tags: ["KOL Campaign", "Content Strategy", "Government"] },
    { title: "NEA Public Hygiene 2024", employer: "Publicis", tags: ["Content Strategy", "KOL Campaign", "Government"] },
    { title: "MSE GoGreenSG 2023", employer: "Publicis", tags: ["KOL Campaign", "Sustainability", "Government"] },
    { title: "MOM Flexible Work Arrangements", employer: "Publicis", tags: ["KOL Campaign", "Content Strategy", "Government"] },
    { title: "Uniform Services Recruitment 2023/2024", employer: "Publicis", tags: ["Content Strategy", "Recruitment", "Government"], links: [{ label: "Instagram", url: "https://www.instagram.com/reels/C-9_C0qStuU/" }, { label: "Facebook", url: "https://www.facebook.com/watch/?v=841938367511619" }] },
    { title: "Energy Market Authority — Net Zero by 2050", employer: "Publicis", tags: ["Content Strategy", "Sustainability", "Government"], links: [{ label: "TikTok", url: "https://www.tiktok.com/@justkeepthinking/video/7323520494689422594" }] },
    { title: "CIMB Hari Raya 2019", employer: "Ogilvy", tags: ["Campaign Execution", "Video", "Financial Services"], links: [{ label: "Campaign Brief Asia", url: "https://campaignbriefasia.com/2019/01/31/celebrations-are-only-perfect/" }, { label: "Business Today", url: "https://www.businesstoday.com.my/2019/05/31/a-grateful-heart-makes-life-meaningful-and-full-of-hope/" }] },
  ],
  awards: [
    { icon: "🥇", title: "GOLD — Content Marketing Excellence", body: "Awarded for SPF's 2025 anti-scam content strategy across multiple scam verticals.", year: "2025 · MEA Singapore" },
    { icon: "🏆", title: "Best Branding Campaign", body: "Won for SCDF's 'What's Your Emergency?' — platform-native behaviour change content.", year: "2024 · TikTok Singapore" },
    { icon: "🥈", title: "SILVER — Brand Awareness Excellence", body: "Awarded for SCDF campaign's measurable impact on public awareness and emergency call behaviour.", year: "2024 · MEA Singapore" },
    { icon: "🥉", title: "BRONZE — Most Effective Use, Gov/Non-Profit", body: "Recognised for effective use of digital channels in the government sector.", year: "2023 · Markies Singapore" },
    { icon: "🎖️", title: "Shortlisted — APPIES Marketing Awards", body: "Shortlisted for the CIMB CNY interactive mobile game — gamification in financial services.", year: "2019 · APPIES Asia Pacific" },
    { icon: "⭐", title: "Top CNY Festive Ad of the Year", body: "Rated a top festive ad of 2019 by Campaign Asia for creative and commercial impact.", year: "2019 · Campaign Asia" },
  ],
};

const colors = {
  black: "#0a0a0a", white: "#f7f7f7", cream: "#ebebeb",
  accent: "#0a0a0a", accent2: "#444444", mid: "#888888",
  border: "rgba(10,10,10,0.15)", cardBg: "#e2e2e2",
};

const s = {
  page: { fontFamily: "'Georgia', 'Times New Roman', serif", background: colors.white, color: colors.black, minHeight: "100vh" },
  nav: { position: "sticky", top: 0, zIndex: 100, display: "flex", justifyContent: "space-between", alignItems: "center", padding: "1rem 3rem", background: colors.white, borderBottom: `1px solid ${colors.border}` },
  navLogo: { fontWeight: 800, fontSize: "0.85rem", letterSpacing: "0.12em", textTransform: "uppercase", color: colors.black, textDecoration: "none", fontFamily: "sans-serif" },
  navLinks: { display: "flex", gap: "2rem", listStyle: "none" },
  navLink: { fontSize: "0.72rem", letterSpacing: "0.1em", textTransform: "uppercase", color: colors.mid, textDecoration: "none", fontFamily: "sans-serif" },
};

function Nav({ active, setActive }) {
  const links = ["Work", "Awards", "Skills", "Contact"];
  return (
    <nav style={s.nav}>
      <a style={s.navLogo} href="#">Portfolio</a>
      <ul style={s.navLinks}>
        {links.map(l => (
          <li key={l}>
            <a href={`#${l.toLowerCase()}`} style={{ ...s.navLink, color: active === l ? colors.accent : colors.mid }}
              onClick={() => setActive(l)}>{l}</a>
          </li>
        ))}
      </ul>
    </nav>
  );
}

function Hero() {
  return (
    <div style={{ minHeight: "60vh", display: "flex", alignItems: "center", padding: "3rem 3.5rem", borderBottom: `1px solid ${colors.border}` }}>
      <div style={{ maxWidth: 680 }}>
        <p style={{ fontSize: "0.7rem", letterSpacing: "0.18em", textTransform: "uppercase", color: colors.accent, fontFamily: "sans-serif", fontWeight: 600, marginBottom: "1.25rem" }}>
          {data.hero.eyebrow}
        </p>
        <h1 style={{ fontFamily: "Georgia, serif", fontSize: "clamp(1.8rem, 3.5vw, 3.2rem)", fontWeight: 700, lineHeight: 1.2, letterSpacing: "-0.02em", marginBottom: "2rem", maxWidth: 640 }}>
          {data.hero.headline}
        </h1>
        <p style={{ fontSize: "1rem", lineHeight: 1.8, color: "#3a3733", maxWidth: 520, marginBottom: "2.5rem", fontWeight: 400 }}>
          {data.hero.bio}
        </p>
        <a href="#work" style={{ display: "inline-flex", alignItems: "center", gap: "0.6rem", background: colors.black, color: colors.white, padding: "0.9rem 1.8rem", fontSize: "0.72rem", letterSpacing: "0.12em", textTransform: "uppercase", textDecoration: "none", fontFamily: "sans-serif", fontWeight: 600 }}>
          View My Work <span>→</span>
        </a>
      </div>
    </div>
  );
}

function Expertise() {
  return (
    <div id="skills" style={{ background: colors.black, color: colors.white, padding: "3rem 3.5rem" }}>
      <p style={{ fontSize: "0.7rem", letterSpacing: "0.2em", textTransform: "uppercase", color: "#cccccc", fontFamily: "sans-serif", fontWeight: 600, marginBottom: "0.75rem" }}>What I Do</p>
      <h2 style={{ fontFamily: "Georgia, serif", fontSize: "clamp(1.8rem, 3vw, 2.6rem)", fontWeight: 700, lineHeight: 1.1, letterSpacing: "-0.02em", marginBottom: "2rem", maxWidth: 580 }}>
        Commercial Marketing Across the Full Growth Funnel.
      </h2>

      {/* Disciplines */}
      <div style={{ display: "grid", gridTemplateColumns: "repeat(4, 1fr)", gap: "2.5rem", paddingBottom: "2rem", borderBottom: "1px solid rgba(255,255,255,0.1)", marginBottom: "2rem" }}>
        {data.expertise.map((e) => (
          <div key={e.num}>
            <div style={{ fontSize: "0.65rem", letterSpacing: "0.2em", color: "#aaaaaa", fontFamily: "sans-serif", fontWeight: 700, marginBottom: "0.85rem" }}>{e.num}</div>
            <div style={{ fontFamily: "Georgia, serif", fontSize: "1rem", fontWeight: 700, lineHeight: 1.3 }}>{e.title}</div>
          </div>
        ))}
      </div>

      {/* Skills lists */}
      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "4rem" }}>
        {[
        { heading: "Commercial Strategy & Growth", items: [
          "Revenue & Growth Marketing",
          "Brand Positioning & Market Entry",
          "Go-to-Market Planning & Execution",
        ]},
        { heading: "Performance & Retention", items: [
          "Paid Media & Performance Optimisation",
          "CRM, Loyalty & Email Marketing",
          "Social Media & Community Growth",
        ]},
      ].map(col => (
          <div key={col.heading}>
            <div style={{ fontFamily: "sans-serif", fontWeight: 700, fontSize: "0.72rem", letterSpacing: "0.12em", textTransform: "uppercase", color: "#aaaaaa", marginBottom: "1.5rem", paddingBottom: "0.75rem", borderBottom: "1px solid rgba(255,255,255,0.15)" }}>{col.heading}</div>
            {col.items.map(skill => (
              <div key={skill} style={{ fontSize: "0.9rem", fontFamily: "sans-serif", color: colors.white, paddingBottom: "0.6rem", marginBottom: "0.6rem", borderBottom: "1px solid rgba(255,255,255,0.07)" }}>
                {skill}
              </div>
            ))}
          </div>
        ))}
      </div>
    </div>
  );
}

function MetricStrip({ metrics }) {
  return (
    <div style={{ display: "flex", flexWrap: "wrap", border: `1px solid ${colors.border}`, background: colors.cream, marginBottom: "1.25rem" }}>
      {metrics.map((m, i) => (
        <div key={i} style={{ flex: "1 1 130px", padding: "1rem 1.4rem", borderRight: i < metrics.length - 1 ? `1px solid ${colors.border}` : "none" }}>
          <div style={{ fontFamily: "Georgia, serif", fontSize: "1.4rem", fontWeight: 700, color: "#222222", lineHeight: 1, marginBottom: "0.3rem" }}>{m.val}</div>
          <div style={{ fontSize: "0.65rem", textTransform: "uppercase", letterSpacing: "0.08em", color: colors.mid, lineHeight: 1.4, fontFamily: "sans-serif" }}>{m.label}</div>
        </div>
      ))}
    </div>
  );
}

function ImpactBadge({ text }) {
  return (
    <div style={{ display: "inline-flex", alignItems: "center", gap: "0.5rem", background: "#222222", color: colors.white, padding: "0.55rem 1rem", fontSize: "0.72rem", letterSpacing: "0.08em", textTransform: "uppercase", fontFamily: "sans-serif", fontWeight: 600, marginBottom: "1.25rem" }}>
      {text}
    </div>
  );
}

function Campaigns() {
  const [hovered, setHovered] = useState(null);
  return (
    <section id="work" style={{ padding: "3rem 3.5rem", background: colors.white }}>
      <p style={{ fontSize: "0.7rem", letterSpacing: "0.2em", textTransform: "uppercase", color: colors.accent, fontFamily: "sans-serif", fontWeight: 600, marginBottom: "0.75rem" }}>Selected Work</p>
      <div>
        {data.campaigns.map((c, i) => (
          <div key={c.num}
            onMouseEnter={() => setHovered(i)}
            onMouseLeave={() => setHovered(null)}
            style={{
              display: "grid", gridTemplateColumns: "52px 1fr", gap: "2rem", alignItems: "start",
              padding: "1.5rem 0", borderTop: `1px solid ${colors.border}`,
              borderBottom: i === data.campaigns.length - 1 ? `1px solid ${colors.border}` : "none",
              background: hovered === i ? colors.cardBg : "transparent",
              transition: "background 0.2s",
              paddingLeft: hovered === i ? "1.25rem" : 0,
              paddingRight: hovered === i ? "1.25rem" : 0,
              marginLeft: hovered === i ? "-1.25rem" : 0,
              marginRight: hovered === i ? "-1.25rem" : 0,
            }}>
            <div style={{ fontFamily: "sans-serif", fontSize: "0.65rem", letterSpacing: "0.15em", color: colors.accent, fontWeight: 700, paddingTop: "0.2rem" }}>{c.num}</div>
            <div>
              <div style={{ fontSize: "0.65rem", letterSpacing: "0.15em", textTransform: "uppercase", color: colors.mid, fontFamily: "sans-serif", fontWeight: 500, marginBottom: "0.45rem" }}>{c.employer}</div>
              <div style={{ fontFamily: "Georgia, serif", fontSize: "1.2rem", fontWeight: 700, lineHeight: 1.25, marginBottom: "0.85rem" }}>{c.title}</div>
              <div style={{ fontSize: "0.875rem", color: "#4a4540", lineHeight: 1.8, maxWidth: 700, marginBottom: "1.25rem", fontFamily: "sans-serif" }}>{c.desc}</div>
              {c.metrics && <MetricStrip metrics={c.metrics} />}
              {c.impact && <ImpactBadge text={c.impact} />}
              <div style={{ display: "flex", flexWrap: "wrap", gap: "0.45rem", marginBottom: c.links ? "1rem" : 0 }}>
                {c.tags.map(t => (
                  <span key={t} style={{ fontSize: "0.62rem", letterSpacing: "0.09em", textTransform: "uppercase", border: `1px solid ${colors.border}`, padding: "0.28rem 0.7rem", color: colors.mid, fontFamily: "sans-serif", fontWeight: 500 }}>{t}</span>
                ))}
              </div>
              {c.links && (
                <div style={{ display: "flex", flexWrap: "wrap", gap: "0.75rem" }}>
                  {c.links.map(l => (
                    <a key={l.label} href={l.url} target="_blank" rel="noopener noreferrer"
                      style={{ display: "inline-flex", alignItems: "center", gap: "0.4rem", fontSize: "0.72rem", fontFamily: "sans-serif", fontWeight: 600, letterSpacing: "0.06em", color: colors.black, textDecoration: "none", borderBottom: `1px solid ${colors.black}`, paddingBottom: "1px" }}>
                      {l.label} ↗
                    </a>
                  ))}
                </div>
              )}
            </div>
          </div>
        ))}
      </div>
    </section>
  );
}

function AdditionalWork() {
  return (
    <section style={{ padding: "3rem 3.5rem", background: colors.white }}>
      <p style={{ fontSize: "0.7rem", letterSpacing: "0.2em", textTransform: "uppercase", color: colors.accent, fontFamily: "sans-serif", fontWeight: 600, marginBottom: "0.75rem" }}>More Work</p>
      <h2 style={{ fontFamily: "Georgia, serif", fontSize: "clamp(1.8rem, 3vw, 2.6rem)", fontWeight: 700, lineHeight: 1.1, letterSpacing: "-0.02em", marginBottom: "2rem", maxWidth: 560 }}>
        Other Campaigns & Projects.
      </h2>
      <div style={{ display: "grid", gridTemplateColumns: "repeat(4, 1fr)", gap: "1px", background: colors.border }}>
        {data.additional.map((c, i) => (
          <div key={i} style={{ background: colors.white, padding: "1.25rem" }}>
            <div style={{ fontSize: "0.62rem", letterSpacing: "0.12em", textTransform: "uppercase", color: colors.mid, fontFamily: "sans-serif", fontWeight: 500, marginBottom: "0.5rem" }}>{c.employer}</div>
            <div style={{ fontFamily: "Georgia, serif", fontSize: "0.95rem", fontWeight: 700, lineHeight: 1.3, marginBottom: "1rem" }}>{c.title}</div>
            <div style={{ display: "flex", flexWrap: "wrap", gap: "0.4rem", marginBottom: c.links ? "1rem" : 0 }}>
              {c.tags.map(t => (
                <span key={t} style={{ fontSize: "0.6rem", letterSpacing: "0.08em", textTransform: "uppercase", border: `1px solid ${colors.border}`, padding: "0.2rem 0.6rem", color: colors.mid, fontFamily: "sans-serif" }}>{t}</span>
              ))}
            </div>
            {c.links && (
              <div style={{ display: "flex", flexWrap: "wrap", gap: "0.75rem" }}>
                {c.links.map(l => (
                  <a key={l.label} href={l.url} target="_blank" rel="noopener noreferrer"
                    style={{ fontSize: "0.68rem", fontFamily: "sans-serif", fontWeight: 600, letterSpacing: "0.06em", color: colors.black, textDecoration: "none", borderBottom: `1px solid ${colors.black}`, paddingBottom: "1px" }}>
                    {l.label} ↗
                  </a>
                ))}
              </div>
            )}
          </div>
        ))}
      </div>
    </section>
  );
}

function Awards() {
  return (
    <section id="awards" style={{ padding: "3rem 3.5rem", background: colors.cream }}>
      <p style={{ fontSize: "0.7rem", letterSpacing: "0.2em", textTransform: "uppercase", color: colors.accent, fontFamily: "sans-serif", fontWeight: 600, marginBottom: "0.75rem" }}>Recognition</p>
      <h2 style={{ fontFamily: "Georgia, serif", fontSize: "clamp(1.8rem, 3vw, 2.6rem)", fontWeight: 700, lineHeight: 1.1, letterSpacing: "-0.02em", marginBottom: "2rem", maxWidth: 560 }}>
        Work That Has Been Recognised by the Industry.
      </h2>
      <div style={{ display: "grid", gridTemplateColumns: "repeat(3, 1fr)", gap: "1px", background: colors.border }}>
        {data.awards.map((a, i) => (
          <div key={i} style={{ background: colors.cream, padding: "1.5rem" }}>
            <div style={{ fontSize: "1.4rem", marginBottom: "1rem" }}>{a.icon}</div>
            <div style={{ fontFamily: "Georgia, serif", fontWeight: 700, fontSize: "0.95rem", marginBottom: "0.5rem" }}>{a.title}</div>
            <div style={{ fontSize: "0.8rem", color: colors.mid, lineHeight: 1.65, fontFamily: "sans-serif", marginBottom: "1rem" }}>{a.body}</div>
            <div style={{ fontSize: "0.65rem", letterSpacing: "0.15em", color: colors.accent, fontFamily: "sans-serif", fontWeight: 700, textTransform: "uppercase" }}>{a.year}</div>
          </div>
        ))}
      </div>
    </section>
  );
}

function Contact() {
  return (
    <div id="contact" style={{ background: colors.black, color: colors.white, padding: "3rem 3.5rem", display: "grid", gridTemplateColumns: "1fr 1fr", gap: "3rem", alignItems: "center" }}>
      <div>
        <h2 style={{ fontFamily: "Georgia, serif", fontSize: "clamp(2rem, 3.5vw, 3.2rem)", fontWeight: 700, lineHeight: 1.1, letterSpacing: "-0.02em", marginBottom: "1.5rem" }}>
          Let's Build Something <span style={{ color: "#aaaaaa" }}>Worth Measuring.</span>
        </h2>
        <p style={{ fontSize: "0.9rem", color: "rgba(245,243,238,0.55)", lineHeight: 1.8, fontFamily: "sans-serif", marginBottom: "1.5rem" }}>
          Open to Brand & Marketing Manager roles across Singapore and the region. I bring strategy, creative direction, and the executional rigour to make campaigns deliver.
        </p>
        <button disabled style={{ display: "inline-flex", alignItems: "center", gap: "0.6rem", background: "transparent", color: "rgba(245,243,238,0.35)", border: "1px solid rgba(245,243,238,0.15)", padding: "0.75rem 1.25rem", fontSize: "0.72rem", letterSpacing: "0.08em", fontFamily: "sans-serif", cursor: "not-allowed" }}>
          Learn more about my personality & characteristics, working style & ethics
          <span style={{ fontSize: "0.65rem", background: "rgba(245,243,238,0.1)", padding: "0.15rem 0.5rem", letterSpacing: "0.1em", textTransform: "uppercase" }}>Coming Soon</span>
        </button>
      </div>
      <div style={{ display: "flex", flexDirection: "column", gap: "1.5rem" }}>
        {[
          { label: "Email", val: "hels.siew@gmail.com", href: "mailto:hels.siew@gmail.com" },
          { label: "LinkedIn", val: "linkedin.com/in/helenasiew", href: "https://www.linkedin.com/in/helenasiew/" },
          { label: "Resume", val: "Download CV", href: "./Helena_Siew_-_Resume_2026.pdf" },
        ].map(l => (
          <a key={l.label} href={l.href} style={{ display: "flex", justifyContent: "space-between", alignItems: "center", color: colors.white, textDecoration: "none", paddingBottom: "1rem", borderBottom: "1px solid rgba(255,255,255,0.1)" }}>
            <div>
              <div style={{ fontSize: "0.62rem", textTransform: "uppercase", letterSpacing: "0.15em", color: "rgba(245,243,238,0.4)", fontFamily: "sans-serif", marginBottom: "0.2rem" }}>{l.label}</div>
              <div style={{ fontSize: "0.9rem", fontFamily: "sans-serif" }}>{l.val}</div>
            </div>
            <span style={{ fontSize: "1.2rem" }}>→</span>
          </a>
        ))}
      </div>
    </div>
  );
}

function Footer() {
  return (
    <footer style={{ background: colors.black, color: "rgba(245,243,238,0.25)", textAlign: "center", padding: "1.5rem 3rem", fontSize: "0.72rem", letterSpacing: "0.08em", fontFamily: "sans-serif", borderTop: "1px solid rgba(255,255,255,0.06)" }}>
      © 2025 · Brand & Marketing Manager · Singapore
    </footer>
  );
}

function Portfolio() {
  const [active, setActive] = useState("Work");
  return (
    <div style={s.page}>
      <Nav active={active} setActive={setActive} />
      <Hero />
      <Expertise />
      <Campaigns />
      <AdditionalWork />
      <Awards />
      <Contact />
      <Footer />
    </div>
  );
}


ReactDOM.createRoot(document.getElementById("root")).render(React.createElement(Portfolio));

</script>
</body>
</html>
