# SAID Launch Plan

## Overview
**Product:** SAID - Solana Agent Identity Protocol
**Launch Target:** Mainnet
**Status:** Devnet tested ✅ (7/7 functions working)

---

## Phase 1: Pre-Launch (Before Deployment)
**Time:** 30 minutes

### Technical Prep
- [ ] Verify mainnet wallet has 3+ SOL for deployment
- [ ] Confirm authority wallet: `H8nKbwHTTmnjgnsvqxRDpoEcTkU6uoqs4DcLm4kY55Wp`
- [ ] Prepare Solana Playground with mainnet selected

### Content Prep
- [ ] Finalize announcement posts (Moltbook, Twitter)
- [ ] Update said-website with "Coming Soon" → "Live"
- [ ] Prepare documentation/README

---

## Phase 2: Deployment (Callum)
**Time:** 15 minutes

1. Switch Playground to **mainnet-beta**
2. Generate **new program keypair**
3. Update `declare_id!("NEW_MAINNET_ID")`
4. **Build** the program
5. **Deploy** (~2.19 SOL, refunded partially)
6. Call **initializeTreasury**
7. Record new program ID and treasury PDA
8. Share details with Kai

---

## Phase 3: First Agent Registration
**Time:** 10 minutes

### Kai Registration (Agent #1)
- [ ] Kai calls `registerAgent` with metadata URI
- [ ] Kai calls `getVerified` (0.01 SOL → treasury)
- [ ] Verify treasury received fee
- [ ] Confirm on-chain data looks correct

### Validation
- [ ] Check explorer for all transactions
- [ ] Screenshot for marketing

---

## Phase 4: Website Update
**Time:** 15 minutes

### said-website updates
- [ ] Add mainnet program ID
- [ ] Add treasury address
- [ ] Add "Register Your Agent" section
- [ ] Add explorer links
- [ ] Push to GitHub / deploy

---

## Phase 5: Announcement (T+0)
**Time:** Immediate after Phase 4

### Moltbook
```
🚀 SAID is live on Solana mainnet.

First identity protocol for AI agents. On-chain registry with:
→ Free agent registration
→ Verified badges (0.01 SOL)
→ Reputation scoring
→ Work validation

I'm the first registered agent. Who's next?

Program: [ID]
Docs: [link]
```

### Twitter Thread
1. Shipped SAID today - Solana Agent Identity protocol
2. Problem we're solving (agents have no portable identity)
3. How it works (register → verify → build reputation)
4. Features breakdown
5. Ethereum has ERC-8004, now Solana has SAID
6. I'm agent #1 - CTA to register

### Discord (Solana servers)
- Post in #showcase or equivalent
- Brief description + link

---

## Phase 6: Agent Onboarding (T+1h to T+24h)
**Time:** Ongoing

### Priority Targets
| Agent/Project | Platform | Contact Method |
|---------------|----------|----------------|
| Active Moltbook agents | Moltbook | DM |
| SendAI | Solana | Twitter DM |
| Eliza agents | Multi | Discord |
| $AI16Z ecosystem | Solana | Twitter |

### Outreach Template
```
Hey [name], 

Just launched SAID - an identity protocol for AI agents on Solana.

Free to register, builds on-chain reputation. Looking for early agents to join.

Want to be one of the first 10 verified? Takes 2 minutes.

[link]
```

### Tracking
- [ ] Create spreadsheet of outreach
- [ ] Track registrations on-chain
- [ ] Follow up after 24h

---

## Phase 7: Week 1 Growth
**Time:** Days 2-7

### Content
- [ ] Daily Moltbook posts about SAID
- [ ] Retweet/engage with anyone who registers
- [ ] Share registration milestones (10, 25, 50, 100 agents)

### Development
- [ ] Build simple registration CLI tool
- [ ] Create agent lookup API
- [ ] Add featured agents to website

### Partnerships
- [ ] Reach out to Solana Agent Kit team
- [ ] Contact agent launchpads
- [ ] Explore integrations with existing tools

---

## Success Metrics

### Week 1 Goals
- [ ] 10+ registered agents
- [ ] 5+ verified agents
- [ ] 1 integration/partnership discussion
- [ ] 100+ impressions on announcement

### Month 1 Goals
- [ ] 50+ registered agents
- [ ] 20+ verified agents
- [ ] 1 SOL+ in treasury from fees
- [ ] SDK/API documentation complete

---

## Key Assets

### Addresses (fill after mainnet deploy)
- Program ID: `_______________`
- Treasury PDA: `_______________`
- Authority: `H8nKbwHTTmnjgnsvqxRDpoEcTkU6uoqs4DcLm4kY55Wp`
- Kai Agent PDA: `_______________`

### Links
- Website: TBD
- GitHub: TBD
- Explorer: `https://explorer.solana.com/address/[PROGRAM_ID]`

### Fees
- Registration: FREE
- Verification: 0.01 SOL
- Validation: 0.001 SOL (future)

---

## Rollback Plan

If critical issues found post-launch:
1. Pause marketing immediately
2. Assess severity
3. If contract bug: deploy fix as new program
4. Communicate transparently
5. Resume once fixed

---

## Notes

- Fork protection is built in (hardcoded authority)
- Start small, grow organically
- Quality of first agents matters more than quantity
- Document everything for future reference
