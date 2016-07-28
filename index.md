---
layout: default
---

# What Daisy Diff offers

One of the most important features of Daisy Diff is the fact that it "understands" HTML tags and will actually look into the text to decide if a node is same for not.

For example assume that a user has changed a single word in a big paragraph. Most XML libraries would just mark the whole paragraph as different. Daisy Diff however will look into the inline text (the contents of the p tag node) and understand that only one word is different. Therefore it will present to the user *only* this word as changed.

DaisyDiff is also used in production (Daisy CMS) and also comes with a business friendly licence.

 * [CustomizingHtmlOutput](CustomizingHtmlOutput)
 * [Examples](Examples)
 * [Papers](Papers)