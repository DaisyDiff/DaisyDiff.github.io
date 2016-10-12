{% comment %}
 This page doesn't have YAML Front Matter block (which would be between ---- and ----). Otherwise, such YAML would show up as page content this when file is included from _layouts/default.md.
This page has to be .md rather than .html, so that we can use it with Markdown Viewer add-on (see https://selite.github.io/DocumentationStandard). Only when it's an .md file, Markdown Viewer automatically changes the local links that don't contain .md extension to contain .md extension. (Otherwise the referenced files won't open locally in Firefox.)

To test links from this webpage with Markdown Viewer on Linux/Mac OS, create a symlink to this file from a folder above.
-->
{% endcomment %}
{% if include.asBootstrapMenu %}
    {% assign topLiClass = 'class="dropdown"' %}
    {% assign luClass = 'class="dropdown-menu"' %}
    {% assign caret = '<span class="caret"></span>' %}
    {% assign menuOpener= '<a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false"' %}
    {% assign menuCloser= '</a>' %}
{% else %}
    {% assign topLiClass = '' %}
    {% assign luClass = '' %}
    {% assign caret = '' %}
    {% assign menuOpener= '<span' %}
    {% assign menuCloser= '</span>' %}
{% endif %}
<li {{ topLiClass }}>
  {{ menuOpener }} data-group-page-names="./ Examples">DaisyDiff{{ caret }}{{ menuCloser }}
  <ul {{ luClass }} role="menu">
    <li><a href="./">Overview</a></li>
    <li><a href="Examples">Examples</a></li>
    <li><a href="Papers">Papers</a></li>
    {% comment %}
        If you'd like a separator between menu items, or a submenu-like header, use:
        <li class="divider"></li>
        <li class="dropdown-header">Internal:</li>
    {% endcomment %}
  </ul>
</li>
<li {{ topLiClass }}>
  {{ menuOpener }} data-group-page-names="Development CustomizingHtmlOutput">Development{{ caret }}{{ menuCloser }}
  <ul {{ luClass }} role="menu">
    <li><a href="Development">Development</a></li>
    <li><a href="CustomizingHtmlOutput">CustomizingHtmlOutput</a></li>
  </ul>
</li>
