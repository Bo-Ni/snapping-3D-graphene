---
layout: post
title: "Lattice design: 1D SCNT and 3D graphene nanolattice"
date: 2019-11-26 21:05:55 +0300
image: Part_III.jpg
tags: "Lattice design"
---

## 1D lattice: straw-like carbon nanotubes (SCNTs)

Straightforwardly, by repeating the unit cell along the axial direction, we obtain the 1D lattice of a straw-like CNT (SCNT). The SCNT sample can have multiple mechanically stable states with different lengths. The force-strain curve shows snap-through events with energy dissipation (Fig. 3 a and b).

![]({{site.baseurl}}/images/figures/fig3.jpg)
*Fig. 3. 1D lattice design: a straw-like CNT. (a) The four stress-free equilibrium configurations with different lengths. (b) Force-strain and potential energy-strain curves during transition from the fully folded stated to the fully extended state under tension via MD. (c) One unit cell compressed back to its folded state without suffering axial buckling. (d) Axial buckling of the SCNT with three unit cells under compression.*


However, it can be hard to transform the extended configuration back to the folded one due to global axial buckling of SCNT under compression. 
* With small axial length, like one unit cell, SCNT can be compressed back (Fig. 3 c)
* As the axial length increases, SCNT buckles along axial direction before snap-through can happen (Fig. 3 d).
This asymmetry in tension and compression limits the reconfigurability of 1D SCNT in cyclic loading. 
Next, we construct a 3D lattice to overcome this limitation. 

## 3D graphene nanolattice: connected SCNT bundles

![]({{site.baseurl}}/images/figures/fig4.jpg)
*Fig. 4. 3D design: 3D graphene nanolattice made of straw-like graphene unit cells. (a) The square lattice structure of SCNT bundles. (b) The covalently bonded connection between neighboring unit cells and topological defect distribution nearby. (c-d) The stress-strain and strain energy density-strain curves of a single unit cell under a tension-compression loop between the folded and extended states. (e-f) The stress-strain and strain energy density-strain curves of a 3D graphene nanolattice with 3-by-3-by-3 unit cells under a tension-compression loop between the folded and extended states.*

3D lattices are construted as the following.
* Parallel 1D SCNTs are assembled into a bundle-like architecture according to a square lattice.
* Neighboring SCNTs are interconnected through covalent bonding

MD simulations demonstrates that these 3D graphene nanolattices can snap forward and backward between the fully folded and extended states under cyclic loading without suffering global buckling or irreversible damage (See Movie M3 and M4), which makes them elastically reconfigurable.


## Deformation modes: Single unit cell vs collective lattice
It should be noted that the number of unit cells along the axial direction can affect the deformation behavior of the 3D graphene nanolattices.
In the case of one single unit cell under cyclic loading
* The mechanical responses along tension and compression paths show very limited differences (Fig. 4 c-d).
* very limited energy dissipation :(
In the case of multiple unit cells,
* Saw-teeth like stress-strain curves are observed.  
* The stress-strain history takes different paths under tension and compression;
* A hysteresis loop appears;
* Energy associated with the loop is dissipated after the cycle.

Intuitively, this hysteresis behavior can be related to the snap-through instability. To systematically explain the relationship between the hysteresis behavior, snap-through instability and multi-stable configurations, a theoretical model is developed in the next section. 

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
