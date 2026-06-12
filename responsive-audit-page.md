Description: fix 1
On mobile (375px), the hero image overflows the screen, causing horizontal scrolling.

Cause:

.hero img {
  width: 1200px;}

Fix Applied:
Changed fixed width to responsive:
.hero img {
  width: 100%;
  height: auto;
}

Description: fix 2
Menu cards do not fit on mobile and tablet screens. They overflow instead of stacking.

Cause:

.card-grid {
  grid-template-columns: repeat(4, 250px);}

Fix Applied:
Made grid responsive:

.card-grid {
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));}


  