| [home page](https://wenjiajian77.github.io/tswd-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Data visualization examples

## Government Debt Across Countries and Years

This heatmap shows how debt-to-GDP ratios varied across countries from 2007 to 2023. Each cell represents one country or aggregate in one year, with color indicating the debt level. Reading across a row reveals changes over time; reading down a column allows comparisons within a year.

<div class='tableauPlaceholder' id='viz1793476757612' style='position: relative'><noscript><a href='#'><img alt='General Government Debt by Country, 2007–2023 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ge&#47;GeneralGovernmentDebtbyCountry20072023&#47;heatmap&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='GeneralGovernmentDebtbyCountry20072023&#47;heatmap' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ge&#47;GeneralGovernmentDebtbyCountry20072023&#47;heatmap&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' />
</object></div>
<script type='text/javascript'>
    var divElement = document.getElementById('viz1793476757612');
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

[View the interactive heatmap on Tableau Public](https://public.tableau.com/views/GeneralGovernmentDebtbyCountry20072023/heatmap)

**Source:** OECD, [General government debt](https://www.oecd.org/en/data/indicators/general-government-debt.html).

---

## How Much Did Government Debt Change?

Most countries shown had higher debt-to-GDP ratios in 2023 than in 2007. Japan recorded the largest increase at 75.0 percentage points, while Israel had the largest decrease at 10.3 percentage points.

For this redesign, I selected the two endpoint years and subtracted each country's 2007 ratio from its 2023 ratio. I used sorted horizontal bars to make the differences easier to compare, with warm colors for increases and cool colors for decreases. Unlike the heatmap, this chart shows the net change directly, but it does not reveal fluctuations between the two years.

<div class='tableauPlaceholder' id='viz1793480666308' style='position: relative'><noscript><a href='#'><img alt='Change in Government Debt by Country, 2007–2023 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ch&#47;ChangeinGovernmentDebtbyCountry20072023&#47;barchart&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='ChangeinGovernmentDebtbyCountry20072023&#47;barchart' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ch&#47;ChangeinGovernmentDebtbyCountry20072023&#47;barchart&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' />
</object></div>
<script type='text/javascript'>
    var divElement = document.getElementById('viz1793480666308');
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

[View the interactive bar chart on Tableau Public](https://public.tableau.com/views/ChangeinGovernmentDebtbyCountry20072023/barchart)

**Reading the chart:** Values show the 2023 debt-to-GDP ratio minus the 2007 ratio, measured in percentage points. A negative value indicates a lower ratio, not necessarily a reduction in the amount of debt. OECD aggregate entries represent groups rather than individual countries.

**Source:** OECD, [General government debt](https://www.oecd.org/en/data/indicators/general-government-debt.html).
