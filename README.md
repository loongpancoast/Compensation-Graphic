# Revenue-Tied Payout Model Calculator

An interactive compensation calculator that demonstrates a revenue-based earning model with dynamic multipliers and backlog management.

## 🎯 What This Does

This calculator helps employees understand how their compensation scales with company revenue through:

- **Revenue Multipliers**: 1.05x to 1.20x based on weekly NET revenue bands
- **Weekly Role Cap**: $250 maximum for current-week KPI bounties
- **Backlog System**: Tracks pre-validation accrued earnings
- **15% Team Envelope**: Hard cap ensuring business solvency
- **Interactive Calculations**: Real-time updates as you adjust revenue and bounties

## 📊 Key Features

1. **Phase-Based Earning Journey**
   - Phase 1: Accrual & Backlog (pre-validation)
   - Phase 2: Validation triggers ($1,000 NET revenue OR 10 orders)
   - Phase 3: Weekly cash payouts begin

2. **Revenue Band System**
   - R3 (50k+): 1.20x multiplier
   - R2 (25k+): 1.10x multiplier
   - R1 (10k+): 1.05x multiplier
   - R0 (0+): 1.00x multiplier

3. **Live Calculator**
   - Adjust weekly NET revenue
   - Input your accrued KPI bounties
   - See real-time breakdown of your potential earnings

## 🚀 How to Use

Simply open `index.html` in any web browser. The calculator is fully self-contained with no dependencies beyond the CDN-hosted libraries (Tailwind CSS).

### Interactive Elements:
- **Weekly NET Revenue**: Adjust to see how revenue bands affect your multiplier
- **Your Accrued KPI Bounties**: Input your earned bounties to calculate potential payout

The calculator automatically shows:
- Team Payroll Envelope (15% of NET revenue)
- Your Current-Week KPI Payout (with multiplier and cap)
- Headroom for Backlog Clearance
- Backlog Catch-Up Pool (10% target)
- Your Total Cash Paid This Week

## 📁 File Structure

```
/
├── index.html          # Main calculator (all-in-one file)
└── README.md          # This file
```

## 🛠️ Technical Details

- **Framework**: Pure HTML/CSS/JavaScript
- **Styling**: Tailwind CSS (via CDN)
- **Fonts**: Inter (via Google Fonts)
- **No Build Process**: Open directly in browser
- **Mobile Responsive**: Works on all screen sizes

## 💡 Use Cases

- Employee onboarding: Understanding compensation structure
- Sales team presentations: Demonstrating earning potential
- Financial planning: Modeling different revenue scenarios
- Transparent compensation: Building trust through clarity

## 🔧 Customization

To modify the calculator constants, edit these values in the `<script>` section:

```javascript
const ENVELOPE_PERCENTAGE = 0.15;        // Team Hard Cap (15%)
const CATCHUP_POOL_MAX_PERCENTAGE = 0.10; // Backlog constraint (10%)
const CURRENT_WEEK_CAP = 250;            // Max weekly role payout
```

To adjust revenue bands, modify the `REVENUE_BANDS` array:

```javascript
const REVENUE_BANDS = [
    { net_revenue_min: 50000, multiplier: 1.20, label: "R3 (50k+)" },
    // ... add or modify bands as needed
];
```

## 📝 License

This is a demonstration calculator. Adapt as needed for your specific use case.

## 🤝 Contributing

This is a standalone mockup. Feel free to fork and customize for your needs!

---

**Last Updated**: October 2025
