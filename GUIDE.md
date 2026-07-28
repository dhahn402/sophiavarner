# Your website, in plain English

Hi Sophia. This is everything you need to know to take care of
**sophiavarner.com** yourself. No code background required. If you get stuck
at any point, text David.

---

## The short version

Your whole website is **one file**, called `index.html`. All the words, all
the links, all the styling live in that one place. When you change it and
save, the live site updates on its own about a minute later.

You don't need to install anything. You edit it in your web browser.

---

## How to change the words on your site

1. Go to **https://github.dev/dhahn402/sophiavarner**
   (that's `github.dev`, not `github.com` — the `.dev` opens the editor)
2. Sign in with your GitHub account if it asks.
3. On the left you'll see a list of files. Click **`index.html`**.
4. Press **Ctrl+F** (Windows) or **Cmd+F** (Mac) and type a few words of the
   sentence you want to change. It'll jump right to it.
5. Type your new words, right over the old ones.
6. Click the **branch icon** in the left sidebar (it looks like a little
   fork in a road, third icon down). Type a short note about what you
   changed — something like `updated my bio` — and click the **checkmark**.

That's it. Give it a minute, then refresh sophiavarner.com.

### The one rule

Only change text that's **between** the angle brackets, not the brackets
themselves.

```
<h3>Social & Content</h3>
    ↑                ↑
    change this stuff, leave these alone
```

If you accidentally delete a `<` or a `>`, that section may disappear from
the page. Don't panic — nothing is ever really lost. See **Undo** below.

### Two characters to avoid

If you want to type an ampersand, type `&amp;` instead of `&`.
If you want to type a less-than sign, type `&lt;` instead of `<`.
Everything else you can type normally.

---

## How to add your photo

Right now there's a placeholder box that says "Photo coming soon" with your
initials. Here's how to swap in a real picture.

**Pick a good one.** Portrait orientation (taller than it is wide), roughly
1000 pixels wide, and under about 400KB so the page stays fast. If it's a
huge photo straight off your phone, run it through
[squoosh.app](https://squoosh.app) first — drag it in, drag the quality
slider down to around 75, download.

**Name it `sophia.jpg`** — all lowercase, no spaces.

**Upload it:**

1. Go to https://github.com/dhahn402/sophiavarner
2. Click **Add file** → **Upload files**
3. Drag `sophia.jpg` in
4. Click **Commit changes**

**Then tell the site to use it.** Open the editor (step 1 above), find the
word `Photo coming soon`, and you'll see a block that looks like this:

```html
<div class="portrait rv">
  <span class="ph">Photo coming soon</span>
  <div>
    <div class="initials">SV</div>
    <div class="cap">Sophia Varner, New Bern, NC</div>
  </div>
</div>
```

Replace that whole block with this:

```html
<div class="portrait rv">
  <img src="sophia.jpg" alt="Sophia Varner, marketer and community builder in New Bern, NC"
       style="width:100%;height:100%;object-fit:cover" />
</div>
```

Save it the same way as before. Done.

> Keep the `alt` text descriptive — that's the sentence screen readers say
> out loud, and Google reads it too.

---

## The one thing still on your to-do list

The **"Leave a Google review"** button currently points at a Google *search*
for Shoreline Socials. It works, but it makes people hunt for the review box
instead of landing on it.

To fix it, get your direct link:

1. Open your **Google Business Profile**
2. Find **Get more reviews** (sometimes under "Ask for reviews")
3. Copy the short link it gives you — it looks like
   `https://g.page/r/SOMETHING/review`

Then in the editor, search for `google.com/search` and replace that whole
web address with your new one. Keep the quote marks around it.

Once that's done, David can make you a QR code that points straight at it —
good for business cards, receipts, or a little sign by the register.

---

## Undo: nothing is ever really broken

Every save is recorded forever, and any of them can be restored.

Go to https://github.com/dhahn402/sophiavarner/commits/main and you'll see
the full history. Click any entry to see exactly what changed — green is
what got added, red is what got removed.

If something looks wrong on the live site and you can't work out why, text
David with roughly when you saved and what you were trying to change. Rolling
back to any earlier version takes him about ten seconds.

**You cannot permanently break this.** Edit freely.

---

## Good to know

**Changes take about a minute.** If you refresh immediately and see the old
version, wait a minute and refresh again. Still old? Hard-refresh with
**Ctrl+Shift+R** (Windows) or **Cmd+Shift+R** (Mac).

**Your phone number appears in four places** — the top button, the hero, the
contact section, and the footer. If it ever changes, search for `2526709264`
and you'll find every one.

**Don't touch the block at the very bottom** that starts with
`<script type="application/ld+json">`. That's the part that tells Google who
you are and what you do, and it's a big part of why you show up in local
search. If it needs changing, that's a David job.

**The share image** (`og.png`) is what people see when your link gets posted
to Facebook or sent in a text. If your branding changes, that image needs to
be remade to match — ask David.

---

## Where things live

| What | Where |
|---|---|
| Your website | https://sophiavarner.com |
| The editor | https://github.dev/dhahn402/sophiavarner |
| History and undo | https://github.com/dhahn402/sophiavarner/commits/main |
| Your agency | https://shorelinesocials.net |
