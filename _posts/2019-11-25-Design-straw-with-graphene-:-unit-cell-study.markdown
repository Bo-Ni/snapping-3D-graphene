---
layout: post
title:  "Design straw with graphene: unit cell that snaps"
date:   2019-11-25 18:05:55 +0300
image:  Part_II_resize.jpg
tags:   Unit cell design
---

The present study is aimed to address the challenge of toughening carbon nanolattice with the potential of snap-through instability in engineering overall material behavior. Through mechanism-inspired structure design, MD simulations and theoretical analysis, we present a novel design of 3D graphene nanolattice with snap-through instability and demonstrate that it can effectively dissipate deformation energy without accumulating irreversible damages via pseudo plastic deformation.

### Unit cell design

We choose 2D graphene as a basis for our nanolattice design due to its outstanding mechanical properties. To adapt to the 2D geometry of graphene, we focus on shell-based designs.

![]({{site.baseurl}}/images/figures/fig1.jpg)
*Fig. 1. Unit cell of shell structure in flexible straws and its nanoscale graphene counterpart engineered via topological design. (a) Geometry of the unit cell structure in straws. (b-c) The fully folded and fully extended states of flexible straws. (d) Phase field crystal simulation of a 2D crystal sample growing on the designed shell surface. (e) The atomic structure of the graphene unit cell with straw-like geometry after MD relaxation and the topological defects distributed at the inner and outer folds.*

At macroscale, numerous applications and studies have presented various examples of shell structures with snap-through instabilities [37-42]. Here, we borrowed inspiration from one of the simplest cases, the flexible straw [43, 44], which can change length by transforming between the folded state and the extended state (Fig. 1 b and c). As shown in Fig. 1 a, the unit cell structure of such a flexible straw is a pair of intersecting conical frustra (the outer frustum, Q-T-P and the inner one, Q-P, intersecting at the folds P and Q). By designing the geometrical parameters of the unit cell, a recent study [45] has demonstrated that both the axially folded state and the extended state can be mechanically stable (Fig. 1 b and c) for elastic shells. Here, we constructed a full-atom model of graphene counterpart to such a unit cell by taking advantage of the methodology of topological design [46-48]. As shown in Fig. 1 d, phase field crystal modeling [49-51] was adopted to simulate the growth of 2D crystal on the designed geometry of the conical frustra. The thermal stability of the obtained crystal structure was validated by relaxing it under an NPT ensemble with Nose-Hoover thermostat [52] at 0 Pa and 300 K for 50 ps using MD (Details of MD simulations can be found in the appendix). The dimensions of the relaxed sample are listed in Fig. 1 e. It should be noted that even through the relaxed model does not fully conform to the designed geometry (Fig. 1 d), the straw-like topology is stably maintained (Fig. 1 e). Further inspection showed that topological defects [46, 53], such as disclinations and dislocations, only concentrate at the connections of the two frustra, accommodating and stabilizing the curvature transition (Fig 1. e). The inevitable presence of topological defects, their residual stress [47] as well as the Van der Walls (VdW) interactions [54] between graphene frustra make the atomic sample different from its counterpart at large scale.

![]({{site.baseurl}}/images/figures/fig2.jpg)
*Fig. 2. The two stress-free stable configurations of the unit cell and the process of a snap-through event. (a) The force-strain and potential energy-strain curves of the unit cell transforming from the folded state to the extended state. (b) Geometry of the two loading-free equilibrium configurations of the unit cell. The two halves of the unit cell are in the folded and extended states, respectively. (c-f) Snapshots of a snap-through event during a tension test in MD simulation. (g) 2D sketch of the deformation process of the inner frustrum during the snap-through process.*

To explore the snap-through instability and possible mechanically stable states of such straw-like unit cells, uniaxial tension tests were performed by applying a constant strain rate of 10^8/s to the simulation box along the axial direction. During the test, a periodic boundary condition was applied along the axial direction and an NVT ensemble with Nose-Hoover thermostat [52] was adopted to maintain a constant temperature of 10 K. The force-strain and potential energy-strain curves are shown in Fig. 2 a. The potential energy curve shows two parabolic-like parts centered around the folded state (State A) and the extended state (State D), indicating both states have positive stiffness. Relaxation and loading tests via MD demonstrated they are mechanically stable. In the transition region, the force curve suffers a non-positive derivative, resulting from the snap-through instability and the corresponding negative incremental stiffness. Through the snap-through instability, the unit cell achieves a 33% elongation without any irreversible damage to the crystal structure (Fig. 2 b). Careful inspection showed that the snap-through event mainly takes place at the inner frustum (P-Q in Fig. 2 b) with the outer frustum (Q-T-P in Fig. 2 b) serving as a constraint to its deformation. At the folded state, the inner frustum is already self-stressed under no external loading (Fig. 2 c). As the external tension increases, the highly compressive stress state is pushed toward the inner fold, Q (Fig. 2 d). At the critical moment, the axial-symmetry of the deformation is broken (Fig 2. e) and the inner frustrum flips out (Fig. 2 f), resulting in a snap-through event (Fig. 2 g). Compared to the folded state (Fig. 2 c), the residual stress in the inner frustrum is reduced in the extended state (Fig. 2 f). Correspondingly, the potential energy in the extended state is lower than that of the folded state (Fig. 2 a) even through the two share the same atomistic topology. In short, the straw-like unit cell possesses two mechanically stable states and can snap-through between them under tension, suffering no permanent damage. It is also interesting to note that similar bi-stable states and snap-through events have been studied in shell systems at macroscale. For example, via experiments and finite element simulations, mirror buckling and snap-through events in spherical cap shells have been studied, where it is demonstrated that the initial asymmetrical buckling can make the snap-through more robust [41]. Recently, an energy landscape analysis is conducted for cylindrical shells. Such detailed energy landscape proved to be an insightful guidance for designing controllable buckling paths between different states [42]. Inspired by these advances in shell buckling study, we wish to point out that it is very likely the straw-like unit cell presented here can be further tuned for more optimized mechanical behavior. For instance, by adjusting its geometrical dimensions, defect/imperfection distributions and residual stress fields, the unit cell may demonstrate a higher stress level for snap-through transition and a larger elongation between the folded and the extended states. We leave this optimization to a future study and focus on the coupling between the unit cell behavior and the lattice level design in the current study.

In the following section, we combine the unit cell with different lattice designs to construct 1D and 3D graphene nanolattices and study their collective deformation behaviors, aiming at engineering effective energy dissipation by leveraging the effect of the snap-through instability.


<!--
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
-->
