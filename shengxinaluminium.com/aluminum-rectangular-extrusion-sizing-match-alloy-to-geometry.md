# Aluminum Rectangular Extrusion Sizing: Match Alloy to Geometry

## The quote is not the finished design

Across extrusion drawing reviews, one failure pattern appears repeatedly: a buyer treats **2 × 1 × 0.125 in, 6063** as a complete material specification. It is not. That description identifies an approximate outside envelope, a nominal wall thickness, and an alloy family. It does not identify the temper, actual mechanical minimums, corner radii, straightness, twist, surface treatment, load direction, or joint condition.

Two profiles can share the same nominal dimensions and behave very differently in service. One may be intended for an anodized architectural frame; another may be selected for a welded machine guard or a load-bearing support. The outside dimensions alone do not make them interchangeable.

Reference material such as a [rectangular extrusion sizing guide](https://www.shengxinaluminium.com/aluminum-rectangular-extrusion-several-alloy-and-sizing-secrets-suppliers-hide_n973) is useful for decoding catalog notation, but a catalog size is only the starting point. The useful engineering insight is that alloy, geometry, and application must be specified as one connected system.

## Build the specification as one connected stack

A predictable rectangular extrusion has several specification layers:

1. **Geometry:** outside width and height, wall thickness, corner radii, internal opening, and any ribs or bridges.
2. **Metallurgy:** alloy, temper, and the mechanical properties guaranteed for that specific section and wall thickness.
3. **Load path:** span, support conditions, bending axis, compression direction, impact, vibration, and connection locations.
4. **Manufacturing limits:** dimensional tolerance, straightness, twist, cut-length accuracy, and variation along the extrusion.
5. **Assembly and environment:** welding, drilling, bolting, coating thickness, temperature changes, corrosion exposure, and visible-surface requirements.

These layers cannot be optimized independently. A thin wall may work when the tube is short and well supported but fail through local buckling in a long compression member. A higher-strength alloy may improve yield margin but do almost nothing for elastic deflection. A nominally correct cavity may not accept a mating insert after wall and coating tolerances are included.

The most expensive purchasing mistakes occur when a supplier is asked to satisfy only the first two items while the design depends on all five.

## Wall thickness changes weight, stiffness, and failure mode together

For a simple rectangular hollow section with sharp corners, the approximate cross-sectional area is:

`A ≈ WH − (W − 2t)(H − 2t)`

Here, `W` and `H` are the outside dimensions and `t` is the wall thickness. A rough weight estimate in pounds per foot is:

`Weight ≈ A × 0.0975 × 12`

The factor 0.0975 represents the approximate density of aluminum in pounds per cubic inch. Actual extrusions vary slightly because corner radii, internal features, and die geometry change the area.

Consider a 2 × 1 × 0.125 in rectangular tube. The idealized cross-sectional area is approximately 0.6875 in², producing a weight of about 0.80 lb per foot. If the wall increases to 0.250 in while the outside size remains unchanged, the area rises to approximately 1.25 in² and the weight to about 1.46 lb per foot. Doubling the wall adds roughly 82% more weight.

The increase in bending stiffness is not identical to the increase in weight. For a 1-in-wide by 2-in-deep section, ignoring corner radii, the strong-axis moment of inertia rises from about 0.332 in⁴ with a 0.125-in wall to about 0.526 in⁴ with a 0.250-in wall. That is approximately a 58% increase in this particular stiffness measure, compared with the 82% increase in weight.

Thicker walls still provide important benefits. They improve resistance to local buckling, increase bearing area around bolt holes, provide more material for tapping, and reduce the risk of burn-through during welding. But the correct wall is not simply the thickest option available. If deflection or weight controls the design, increasing the outside depth or adding a support may deliver more useful performance than adding material near the neutral axis.

This is why a supplier's standard wall chart cannot substitute for a section calculation. The same outside size can represent a lightweight trim profile, a moderate frame member, or a heavy-duty connection component depending on the wall and internal geometry.

## Alloy and temper determine what the section can tolerate

6061 and 6063 are both common 6000-series extrusion alloys, but they solve different problems.

- **6061-T6** is commonly selected when higher structural strength, machinability, and load-bearing performance matter. Representative extrusion data often place its yield strength in the roughly 30–40 ksi range, depending on product form, thickness, and specification.
- **6063-T5 or 6063-T6** is often selected for complex shapes, smooth surfaces, and anodized architectural work. Its typical yield strength is lower, often in the mid-20s to low-30s ksi range, depending on temper and section details.

Those ranges are useful for comparison, not for final design. The certified minimum for the actual profile, wall thickness, alloy, and temper controls. A supplier that lists only 6061 or 6063 without the temper has not provided a complete mechanical specification.

The temper is equally important. T5 generally means the extrusion was artificially aged after cooling from the extrusion process. T6 involves solution heat treatment followed by artificial aging and normally provides higher strength. T6 is not automatically better for every application because it can reduce formability and complicate fabrication.

Welding creates another coupling between metallurgy and geometry. A 6061-T6 mill certificate describes the material before welding. The heat-affected zone next to a weld does not retain the full T6 strength unless a qualified post-weld treatment or a reduced-strength design basis is used. A thin wall may also lose more practical strength through distortion or burn-through than the alloy selection suggests.

Alloy selection also has a limit that is often overlooked: 6061 and 6063 have nearly the same elastic modulus, approximately 10 million psi. Switching from 6063 to 6061 can increase yield strength, but it will not materially eliminate sag under a normal elastic load. If deflection governs, section depth, orientation, span, and support are usually more influential than the alloy upgrade.

## Orientation can matter more than the alloy label

A rectangular tube is directional. Its longer outside dimension should normally be aligned with the direction that requires the greatest bending resistance.

For an idealized rectangular tube, the strong-axis moment of inertia can be estimated with:

`I = [WH³ − (W − 2t)(H − 2t)³] / 12`

Take a 2 × 4 × 0.125 in tube with the 4-in dimension vertical. Ignoring corner radii, its cross-sectional area is about 1.4375 in², its weight is about 1.68 lb per foot, and its strong-axis moment of inertia is approximately 2.98 in⁴. Rotate the same tube 90 degrees and the relevant moment of inertia falls to about 0.99 in⁴.

That is a three-to-one difference in bending stiffness without changing the alloy, wall, mass, or purchase price.

A simple beam example makes the effect tangible. Assume a 48-in simply supported span with a 500-lb point load at the center. Using an elastic modulus of 10,000,000 psi:

- With the 4-in dimension vertical, the estimated center deflection is about 0.039 in and the bending stress is about 4.0 ksi.
- With the tube rotated, the estimated center deflection is about 0.116 in and the bending stress is about 6.0 ksi.

These are simplified elastic estimates, not allowable load ratings. They exclude safety factors, local buckling, holes, connection flexibility, impact, and support distortion. The important comparison is the change caused by orientation. A stronger alloy might improve the yield margin, but it would not turn the second orientation into the first one for deflection purposes.

This is why a tube that is technically strong enough can still be rejected in service because it vibrates, sags, or fails to maintain alignment. The load path must appear on the drawing, not remain an assumption in the installer's head.

## Nominal dimensions hide a tolerance stack

Rectangular tube dimensions are generally described by outside width × outside height × nominal wall thickness. A nominal 2 × 1 × 0.125 in tube therefore has an idealized internal opening of 1.750 × 0.750 in. That opening is not automatically a guaranteed finished clearance.

The relationship is simple:

`Internal width = outside width − 2 × wall thickness`

Small variations in both terms move in the same unfavorable direction. For example, suppose a nominal 2.000-in outside width arrives at 1.980 in and the nominal 0.125-in wall measures 0.135 in. The resulting idealized internal width is only 1.710 in, which is 0.040 in below the nominal 1.750 in opening.

Those values are illustrative, not a statement of the permitted limit for a particular standard. The lesson is tolerance stacking. The actual allowable variation depends on the profile, wall, alloy, temper, tolerance class, and applicable extrusion standard such as ASTM B221 or B221M.

Corner radii make the fit question more complicated. A component may fit between the flat internal faces but interfere at the corners. Internal die bridges or longitudinal weld areas can also matter when the cavity is used for a cable, insert, bearing, or sliding component.

Straightness and twist deserve equal attention. A long extrusion can meet width and height requirements at several measured points yet still fail to assemble into a square frame. For a visible frame, twist creates inconsistent joints and uneven glazing gaps. For a machine structure, it can transfer unintended loads into bearings or fasteners.

A practical drawing should identify critical dimensions rather than demanding unnecessarily tight tolerances everywhere. Ask the supplier to measure the critical outside dimension, wall, internal opening, straightness, and twist using a defined method. Tightening every tolerance increases cost; tightening the dimensions that control function prevents rework.

## Finish and joining complete the specification

Surface treatment is not merely a color decision. It can affect fit, corrosion resistance, appearance, and the way the extrusion must be handled during fabrication.

6063 is often preferred when a visible anodized surface is important because it extrudes smoothly and produces a consistent decorative finish. 6061 can also be anodized or powder coated, but the as-extruded surface may show more die lines or handling marks. A coating can improve protection without correcting a poor surface that was already present.

Powder coating commonly adds a few mils to each coated face, while anodizing also changes the usable surface dimension. A close-fitting insert or sliding part therefore needs a finished, coated clearance rather than a bare-metal clearance. Masking areas, coating thickness, and the required visible face should be included in the order.

Connections expose the same alloy-and-sizing issue. A 0.062-in wall may be adequate for a light enclosure but insufficient for a concentrated bolt load. A washer, insert, sleeve, or thicker local feature may be needed to prevent bearing failure and pull-through. Drilled holes also remove section area and can initiate local buckling near a support.

A hollow extrusion should not be assumed to be pressure-rated simply because it looks like tubing. Profiles made through a porthole die may contain longitudinal seam welds, and pressure service requires a design basis and testing appropriate to the application.

## Write the order so different quotes are genuinely comparable

A usable specification might read:

`2.000 × 4.000 × 0.125 in outside dimensions; 6061-T6; ASTM B221; 48.000 in cut length ±0.062 in; 4.000-in side vertical in service; minimum clear opening stated on drawing; approved corner radii; mill finish; mill test report by heat or lot.`

Additional requirements should be added according to the governing risk:

- For a structural member, state span, support conditions, design load, bending axis, and allowable deflection.
- For a close fit, state the minimum internal opening, maximum external dimension, corner clearance, and finished coating condition.
- For a welded assembly, state the welding process, filler, inspection level, and strength basis for the heat-affected zone.
- For an anodized or powder-coated part, identify coating type, thickness, color, visible surfaces, masking, and sample approval.
- For long members, state straightness, twist, cut-length tolerance, and how those characteristics will be inspected.
- For traceable industrial work, require alloy, temper, lot identification, and certified mechanical or chemical documentation.

Consider three quote lines that appear similar:

- 6063-T5, 2 × 4 × 0.125 in, clear anodized
- 6061-T6, 2 × 4 × 0.125 in, mill finish
- 6061-T6, 2 × 4 × 0.094 in, mill finish

None is an automatic substitute for the others. The first may be the better choice for a visible non-load-bearing frame. The second may provide greater base-metal strength for an unwelded structural member. The third weighs less but has a different section area, bending stiffness, connection capacity, and local-buckling risk. Comparing only price per foot hides those differences.

The correct comparison is finished performance per installed part, not alloy name or nominal size in isolation.

## The rule that prevents false equivalence

The right question is not which alloy has the highest published strength or which supplier offers the lowest price for a nominal size. The right question is which complete specification keeps the governing limit inside the required margin.

- If **strength** governs, match section geometry, alloy, temper, and connection design.
- If **deflection** governs, prioritize depth, orientation, span, and support because common aluminum alloys have similar stiffness.
- If **fit** governs, control actual cavity dimensions, corner radii, tolerances, and coating thickness.
- If **weight** governs, calculate cross-sectional area and compare the stiffness gained per pound.
- If **appearance** governs, specify alloy, extrusion surface, finish, visible faces, and sample approval.
- If **welding** governs, design around the post-weld condition rather than the untouched mill certificate.

A rectangular extrusion is properly specified only when its dimensions, metallurgy, orientation, tolerances, finish, and connection condition appear together on the drawing and purchase order. Without that complete chain, same-size means only same-size on paper—not same performance in the field.

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
- [Rectangular Tube Aluminum Extrusions: Pick The Right ...](https://www.shengxinaluminium.com/rectangular-tube-aluminum-extrusions-pick-the-right-alloy-size-and-finish_n943)
- [Aluminum Tube Extrusions Decoded: Alloys,Shapes,And ...](https://www.shengxinaluminium.com/aluminum-tube-extrusions-decoded-alloys-shapes-and-specs-that-matter_n725)
- [Rectangular Aluminum Extrusions: From Alloy Selection To ...](https://www.shengxinaluminium.com/rectangular-aluminum-extrusions-from-alloy-selection-to-perfect-fit_n761)
- [Aluminum Tube Extrusion Decoded: Alloys,Profiles,And ...](https://www.shengxinaluminium.com/aluminum-tube-extrusion-decoded-alloys-profiles-and-sourcing-secrets_n940)
- [Aluminum Extrusion Pipe Vs Standard Tubing](https://www.shengxinaluminium.com/aluminum-extrusion-pipe-vs-standard-tubing-why-engineers-are-switching_n713)
- [Aluminum Extrusion Tolerances Chart: Stop Overspecifying ...](https://www.shengxinaluminium.com/aluminum-extrusion-tolerances-chart-stop-overspecifying-your-designs_n789)
- [Aluminum Section Decoded Before You Spec,Source,Or ...](https://www.shengxinaluminium.com/aluminum-section-decoded-before-you-spec-source-or-overspend_n670)
- [What Is Extruded Aluminum? Your Definitive Guide to Uses ...](https://www.shengxinaluminium.com/what-is-extruded-aluminum-your-definitive-guide-to-uses-benefits_n306)
- [T Slot Aluminum Extrusion Sizes Decoded: Stop Guessing, ...](https://www.shengxinaluminium.com/t-slot-aluminum-extrusion-sizes-decoded-stop-guessing-start-building_n526)
- [Square Aluminum Extrusion Decoded: From Alloy ...](https://www.shengxinaluminium.com/square-aluminum-extrusion-decoded-from-alloy-selection-to-final-build_n961)