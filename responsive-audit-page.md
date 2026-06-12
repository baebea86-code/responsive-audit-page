Description: fix 1
On mobile (375px), the hero image overflows the screen, causing horizontal scrolling.

Cause:
.hero img {
  width: 1200px;}

Fix Applied:
Changed fixed width to responsive:
.hero img {
  width: 100%;
  height: auto;}
  

Description: fix 2
Menu cards do not fit on mobile and tablet screens. They overflow instead of stacking.

Cause:
.card-grid {
  grid-template-columns: repeat(4, 250px);}

Fix Applied:
Made grid responsive:

.card-grid {
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));}


 Description: fix 3
Contact form does not fit on smaller screens and creates layout overflo

Cause:
.contact-inner {
  width: 800px;}

Fix Applied:
.contact-inner {
  width: 100%;
  max-width: 800px;
  padding: 0 16px;} 