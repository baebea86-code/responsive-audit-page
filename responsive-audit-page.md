Description:
On mobile (375px), the hero image overflows the screen, causing horizontal scrolling.

Cause:

.hero img {
  width: 1200px;
}

Fix Applied:
Changed fixed width to responsive:

.hero img {
  width: 100%;
  height: auto;
}