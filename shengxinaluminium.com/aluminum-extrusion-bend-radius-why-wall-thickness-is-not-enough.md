# Aluminum Extrusion Bend Radius: Why Wall Thickness Is Not Enough

## The radius multiplier is only a screening shortcut

Rules such as 1–3 times wall thickness or 5–10 times wall thickness survive because they are convenient. They can screen a simple, uniform section, but they are not a physical law for every aluminum extrusion.

The missed variable is the distance from the neutral axis to the farthest fiber in the plane of bending. Wall thickness affects local cracking and buckling, but the overall section depth controls how much the outer surface must stretch as the extrusion curves. A practical [aluminum radius design guide](https://www.shengxinaluminium.com/bending-aluminum-extrusions-radius-formulas-engineers-miss_n1017) can provide useful starting equations, but those equations become defensible only after the actual profile geometry and forming process are known.

> The minimum bend radius is not a constant printed on an alloy data sheet. It is the smallest released radius that keeps the most highly strained and least supported part of one defined profile inside a qualified process window.

That distinction explains why a radius that works for a 2 mm flat strip may be impossible for a 2 mm-wall hollow extrusion, even when both parts use the same alloy.

## Why wall thickness gives the wrong answer for many profiles

When an extrusion bends along its length, every point in the cross-section follows a different path. The surface on the outside of the curve stretches, the inside surface compresses, and the section may distort as it moves through the tooling.

Consider two parts with a nominal 2 mm wall and the same 10 mm inside radius.

- A 2 mm flat strip has a centerline radius of roughly 11 mm. Its outer fiber is about 1 mm from the neutral axis, producing a first-pass tensile strain of approximately 1 ÷ 11, or 9.1 percent.
- A 40 mm-deep hollow extrusion with the same 10 mm inside radius has a centerline radius of roughly 30 mm. Its outer fiber is about 20 mm from the neutral axis, producing approximately 20 ÷ 30, or 66.7 percent strain.

The two parts have the same wall-thickness ratio of 5t, but their global bending demand is completely different. The second calculation is far outside the range normally used for a controlled cold-forming design in architectural or structural aluminum.

Neither estimate certifies a material by itself. The contrast exposes the problem with applying a wall-thickness rule without identifying the bend plane and the section depth. Rotate the same extrusion 90 degrees and the distance from the neutral axis changes again; the feasible radius can change substantially without changing the alloy, wall thickness, or nominal bend callout.

An aluminum extrusion is not sheet stock with decorative geometry added. For longitudinal bending, the entire cross-section participates in the curvature.

## The strain calculation behind a defensible first pass

For an initial engineering estimate, treat the centroidal path as an approximation of the neutral-axis path. The outer-fiber strain can then be estimated as:

> outer-fiber strain ≈ y_outer ÷ R_centerline

That gives a minimum centerline radius of:

> minimum R_centerline ≈ y_outer ÷ ε_design

If the radius is specified at the inside surface, convert it using the distance from the neutral axis to the inner surface:

> minimum R_inside ≈ minimum R_centerline − y_inner

Here, y_outer is the distance from the neutral axis to the farthest tension-side fiber, y_inner is the distance to the inside surface, and ε_design is the allowable forming strain for the actual alloy, temper, surface condition, and process.

For a symmetric section with total radial depth h, the first-pass equation becomes:

> minimum R_inside ≈ (h ÷ 2) × (1 ÷ ε_design − 1)

For a flat strip, h is the material thickness, which is why thickness multipliers appear in fabrication references. The multiplier is simply a different way of expressing the selected design strain. At a 10 percent design strain, the calculated inside radius is about 4.5t. At 20 percent, it is about 2t. At 5 percent, it is about 9.5t.

The multiplier changes because the allowable strain changes. It is not a universal property of aluminum.

### A worked extrusion example

Take a nominally symmetric extrusion that is 40 mm deep in the radial direction. Assume qualification work supports an 8 percent design strain for the selected alloy, temper, and bending process.

- The outer-fiber distance is approximately 20 mm.
- The minimum centerline radius is approximately 20 ÷ 0.08, or 250 mm.
- The corresponding inside radius is approximately 250 − 20, or 230 mm.
- The outside radius is approximately 270 mm.

The 8 percent value is an assumption for the example, not a universal aluminum limit. A more formable alloy, a different temper, stretch bending, or a profile with a smaller radial depth could produce a different result. The calculation is valuable because it makes the governing geometry visible before tooling is ordered.

At tight plastic bends, the neutral axis can shift, the wall can thin, and the cross-section can deform. Those effects make the equation a screening tool rather than a final certification method. They do not make the geometry irrelevant; they make physical qualification more important.

## Alloy and temper change the allowable strain, not the geometric term

Alloy selection affects ε_design, but it does not change the distance from the neutral axis to the outer fiber. That is why changing alloy can improve a bend without fixing a fundamentally undersized radius.

- 6063-T5 is often selected for architectural curves because it generally offers more forming margin than stronger 6XXX tempers.
- 6061-T6 provides higher structural strength but is less forgiving at tight radii. The same profile can crack in 6061-T6 after passing in 6063-T5.
- 5052 is frequently considered when tight forming and corrosion resistance matter more than the strength level of a heat-treated 6XXX alloy.
- T4 or annealed conditions can improve formability, but natural aging, final strength, and dimensional consistency must be controlled if the part will later be aged or heat-treated.

A tensile-test elongation from a material datasheet should not be inserted directly as ε_design. A standard tensile specimen has a different stress state and surface condition from the outside of an extrusion moving around a die. Profile bending can also involve directional properties from extrusion, local thinning, corner stress concentrations, surface scratches, and friction against tooling.

A better sequence is to use published material data for screening, apply a conservative margin, then qualify the actual profile in the actual extrusion direction and temper. If the required radius remains too tight, the credible options are to increase the radius, reduce the section depth, add generous profile corner radii, change the alloy or temper, or use a qualified bend-and-age process. Uncontrolled heating is not a substitute for a radius calculation because it can change strength and repeatability along the part.

## Hollow profiles have a second radius limit

The global strain calculation answers only one question: will the outermost fiber stretch too far? Hollow profiles introduce another question: can the compressed side and the unsupported walls maintain their shape while the part bends?

A thin inner wall may wrinkle even when the outer tension strain is acceptable. A tube may ovalize, a chamber may collapse, or a long flat flange may buckle between supporting webs. These failures depend on wall thickness, unsupported width, the width-to-thickness ratio, chamber geometry, corner radii, friction, and the support provided by the tooling.

A useful engineering model is:

> required radius = the maximum of the strain radius, stability radius, and process radius

This is not a code equation. It is a way to prevent a strain-only calculation from being mistaken for a production limit.

For example, two profiles may both measure 40 × 20 mm and have 2 mm outer walls. A rounded single-chamber section may remain stable during a qualified bend, while a similar-looking section with a 0.8 mm internal web and a long unsupported flange may wrinkle at the same radius. The outer-fiber calculation is nearly identical, but the local stability limit is not.

Tooling changes that second limit. A mandrel and wiper die can support thin-wall hollow profiles during rotary draw bending. Stretch bending keeps the section under tension and can reduce compression-side wrinkling on large-radius curves. Roll bending may be effective for long sweeps but can require multiple passes and careful springback control. Ram or press bending may be economical for simple shapes while allowing more cross-section distortion.

The defect often identifies the governing limit:

- Cracks on the outside usually indicate excessive tensile strain, an unsuitable temper, a sharp local corner, or surface damage.
- Wrinkles on the inside usually indicate insufficient support, excessive compression, poor friction control, or an unsupported wall that is too slender.
- A clean profile with the wrong final radius usually indicates springback or an ambiguous radius reference.

## Radius conventions and springback can invalidate correct math

A radius callout is incomplete unless it states what surface or path it references.

- Inside radius is measured to the innermost surface of the bend.
- Centerline radius is measured along the profile centroid path or the industry-defined centerline.
- Outside radius is measured to the outermost surface.

For a 40 mm-deep symmetric section, an inside radius of 230 mm corresponds approximately to a 250 mm centerline radius and a 270 mm outside radius. If a supplier quotes 250 mm without naming the reference, the apparent agreement may conceal a 20 mm difference in geometry.

The tool radius and the released-part radius are also different values. Aluminum stores elastic energy during forming and partially straightens when the tooling opens. Higher-strength tempers often produce more springback, and large-radius bends can show noticeable changes in angle and radius after release.

The drawing should specify the final radius after springback, not only the radius machined into the die. Overbending can compensate for elastic recovery, but the overbend itself raises the peak strain. A crack-prone design cannot be rescued safely by adding more overbend.

Surface finish can create another practical radius limit. Bare metal may survive a bend while a pre-anodized surface develops visible crazing on the tension side. If appearance matters, the qualified radius must pass both the metal-forming criteria and the finish criteria.

## A qualification sequence that turns the formula into a production limit

A reliable radius specification can be developed in seven steps:

1. Freeze the profile drawing, actual minimum wall thicknesses, extrusion direction, bend plane, and section orientation.
2. State whether the required radius is inside, centerline, or outside, and whether it is measured before or after springback.
3. Calculate the outer-fiber strain using the section depth in the radial direction rather than substituting wall thickness automatically.
4. Select a conservative design strain based on alloy, temper, surface condition, and available material data.
5. Check local stability for hollow chambers, thin webs, long unsupported flanges, and corner transitions. Select mandrels, wipers, stretch tooling, or other support where necessary.
6. Run samples using production-intent material and tooling at the target radius and nearby radii. Inspect the outside surface, inside compression zone, section shape, wall thinning, radius, angle, and finish.
7. Set the production limit at the smallest tested radius that passes the acceptance criteria with a documented process margin.

A qualification sample should be evaluated after it has been released from the tooling and, when relevant, after anodizing, powder coating, or another finish. Measuring only the part while it is clamped can hide springback and surface defects that appear later.

## What belongs on the bend drawing

A complete aluminum extrusion bend callout should identify:

- Alloy and temper, including any bend-before-aging requirement
- The section drawing and the orientation of the bend plane
- Inside, centerline, or outside radius reference
- Final radius, bend angle, tangent lengths, and dimensional tolerances after release
- Acceptance limits for cracks, wrinkles, ovality, wall thinning, and visible tool marks
- Required mandrel, wiper, stretch, or roll-bending process when the profile is sensitive
- Surface-finish sequence and appearance requirements

The strongest replacement for a vague 5t rule is a question: which fiber or wall reaches its forming limit first, and what released radius keeps that location inside the qualified process window? Once that question is answered, the radius is no longer a guess based on wall thickness. It becomes a traceable engineering limit tied to the actual extrusion.

## Related Articles

- [Aluminum Extrusion Design: Why the Die Decides Quality Before the Press Runs](https://sites.google.com/view/gs-77efe8198de7ec75)
- [Extrusion Die Design: The Hidden Control Point Behind Aluminum Profile Quality](https://justpaste.it/h2nk1/pdf)
- [Aluminum Extrusion Die Design: The Hidden Control Point for Quality Profiles](https://bsky.app/profile/asdfasdfasdfeq.bsky.social/post/3mv5s7cysyl25)
- [Aluminum Extrusion Design: Why Metal Flow Decides Profile Quality](https://substack.com/profile/545243856-shengxinaluminium/note/c-333813974)
- [Extrusion Die Design: The Hidden Lever Behind Aluminum Profile Quality](https://pad.riseup.net/p/r.58a8dc4b78a527a6caad98b1164c8365)
- [Aluminum Extrusion Die Design Drives Profile Quality](https://dev.to/q0ago/aluminum-extrusion-die-design-drives-profile-quality-2e3h)
- [Aluminum Extrusion Design: Why Metal Flow Decides Quality](https://rentry.co/fz4xmmro)
- [Aluminum Extrusion Die Design: The Hidden Driver of Profile Quality](https://sakthongchanthavong.gitlab.io/posts/aluminum-extrusion-die-design-the-hidden-driver-of-profile-quality)
- [Aluminum Extrusion Die Design: The Hidden Lever Behind Profile Quality](https://gist.github.com/martinwesley85/5c26cf2d297bf74a76db142608cff82a)
- [Aluminum Extrusion Die Design: Why Metal Flow Decides Quality](https://bin.disroot.org/?bf1e093315a6bb28#FNmsavBgnfMd1vA8GgeUPmtLmkCew1sLJKkduV21NFwy)
- [How To Bend Aluminum Extrusions Without Cracking Or ...](https://www.shengxinaluminium.com/how-to-bend-aluminum-extrusions-without-cracking-or-wrinkling_n822)
- [Aluminum Extrusion Bending Demystified: From Defects To ...](https://www.shengxinaluminium.com/aluminum-extrusion-bending-demystified-from-defects-to-flawless-curves_n948)
- [Optimal Methods For Aluminum Extrusion Bending](https://www.shengxinaluminium.com/optimal-methods-for-aluminum-extrusion-bending-choose-right-bend-once_n539)
- [Four-Roll Aluminum Extrusion Bending: Solve Springback ...](https://www.shengxinaluminium.com/four-roll-aluminum-extrusion-bending-solve-springback-before-it-ruins-your-project_n641)
- [Aluminum Extrusion Bending Machine Selection: Match Your ...](https://www.shengxinaluminium.com/aluminum-extrusion-bending-machine-selection-match-your-profile-complexity_n872)
- [Aluminium Bending: The Choices That Decide Clean Or Cracked ...](https://www.shengxinaluminium.com/aluminium-bending-the-choices-that-decide-clean-or-cracked-parts_n583)
- [How To Bend Aluminum Pipe Without Kinks,Cracks,Or ...](https://www.shengxinaluminium.com/how-to-bend-aluminum-pipe-without-kinks-cracks-or-guesswork_n580)
- [News](https://www.shengxinaluminium.com/news_nc1_78)
- [News](https://www.shengxinaluminium.com/News_nc1_13)
- [Shengxin Aluminum Profile Bending Reliable and Customizable](https://www.shengxinaluminium.com/shengxin-aluminum-profile-bending-reliable-and-customizable_p959.html)