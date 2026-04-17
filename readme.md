cd vignelli-agency && cat > README.md << 'EOF'
# Vignelli Agency Design System

A design system for Ext. Marketing, grounded in the principles of Massimo Vignelli's Canon.

## Philosophy

This system is built on three interlocking principles drawn directly from the Vignelli Canon:

**Semantics** — every design decision has a reason. Colour is used as a signifier or identifier, not decoration. Typography organises information objectively. Components mean something before they look like something.

**Syntactics** — consistency is non-negotiable. The grid governs layout. Type scales follow fixed relationships. No element sits arbitrarily on a page.

**Pragmatics** — if it isn't understood, it has failed. Every component must stand alone without explanation.

## Brand Palette

| Token | Hex | Purpose |
|---|---|---|
| Near-black | `#241F21` | Headers, reversed text, primary dark surfaces |
| Gold | `#FFD100` | Primary identifier/accent — signifier only, not decoration |
| Orange | `#FE863C` | Secondary accent |
| Light blue | `#CCE1E4` | Table fills, callout backgrounds |
| Warm off-white | `#EAE8E3` | Secondary fills, section backgrounds |
| Cream | `#F7F3EF` | Page backgrounds |
| Light yellow | `#EBDFA3` | Highlight fills |

## Typography

- **Primary:** Aptos (Microsoft system font)
- **Fallback:** Calibri, then system sans-serif
- Sentence case throughout — no title case, no all-caps headlines
- Flush left as the default alignment
- Maximum two type sizes per component; weight (bold/regular) handles hierarchy within that constraint
- No decorative type use; no type deformation

## Grid

- Grid-first layout at all scales
- Narrow margins preferred to create tension between content and page edge
- Modules divide pages horizontally; columns divide vertically
- All element placement must reference the grid — no arbitrary positioning

## Principles in practice

- Timeless over trendy: no component should read as a product of a particular year
- White space is structural, not cosmetic
- Identity and diversity in balance: consistent identifiers (logo, colour, type) with enough variation to sustain attention
- Economy of means: the leanest solution that fully solves the problem

## Voice and writing style

- Canadian English spelling throughout
- No em-dashes — rewrite the sentence, use a comma, or use a colon
- No Oxford comma except to prevent ambiguity
- Plain, direct language — no marketing inflation

## Stack

- React (functional components, hooks)
- Tailwind CSS (core utility classes only)
- Fonts loaded via system stack or Google Fonts fallback

## References

- Vignelli, Massimo. *The Vignelli Canon*. Lars Müller Publishers, 2010.
- Ext. Marketing brand specification (`ext-docs-artifacts` skill)
EOF
git add README.md && git commit -m "Initial commit: Vignelli-informed design system" && git push -u origin main
