[home page](https://wenjiajian77.github.io/tswd-portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three)

# Critique by Design: Pet Ownership Across Countries and Regions

For this project, I redesigned a visualization about international pet ownership. My goal was to make comparisons within each pet category easier while highlighting how the United States compares with other countries and regions. I developed the redesign through an initial critique, Tableau sketches, classroom feedback, and revisions.

## Step one: the visualization

I selected the pet ownership infographic featured in NielsenIQ’s article, [“Man’s best friend: Global pet ownership and feeding trends.”](https://nielseniq.com/global/en/insights/report/2016/mans-best-friend-global-pet-ownership-and-feeding-trends/) The infographic presents GfK survey results for dogs, cats, fish, and birds across 22 markets.

![Original pet ownership infographic from GfK, published by NielsenIQ](https://nielseniq.com/global/en/wp-content/uploads/sites/4/2024/09/pet_ownership_countries_study_2016.jpg)

*Source: GfK (2016), published by NielsenIQ.*

I chose this visualization because pets are a familiar topic, but ownership patterns vary considerably across countries and regions. The data support questions that both general readers and people working in the pet industry might find interesting: Where is each pet type most common? How does the United States compare with the leaders?

The original infographic caught my attention through its pet icons, colors, and central globe. However, answering those questions required scanning many individual percentages. This made it a useful redesign opportunity: I could retain the approachable subject while making the comparisons more immediate.

## Step two: the critique

I completed the Google Form using Stephen Few’s Data Visualization Effectiveness Profile. The framework helped me consider usefulness, completeness, perceptibility, truthfulness, intuitiveness, aesthetics, and engagement separately.

The original visualization has several strengths. Its pet icons make the categories recognizable, its numerical labels provide exact percentages, and its source information gives readers context. The central summary percentages also offer a starting point for understanding the overall picture. I interpreted its primary audience as pet-industry marketers, retailers, and consumer researchers, with general readers as a secondary audience.

However, the design functions more like an illustrated table than a chart that supports quick comparisons. The central globe occupies considerable space without showing the locations of individual observations. Countries are not ordered by ownership percentage, so readers must search for the largest values. The different arrangements of country names and percentages on the two sides also interrupt the reading flow.

I also wanted the meaning of the percentages to be more prominent. They describe respondents reporting a particular pet type in their household, rather than the number of pets owned. The survey context and the calculation of the overall averages are not easy to assess from the main graphic alone. For professional readers, the data provide an overview, but they do not establish market size or spending potential.

Using Few’s framework helped me distinguish an attractive presentation from an effective comparison tool. Compared with my earlier Good Charts exercises, it encouraged a more systematic review of individual design qualities. However, the categories sometimes overlap, and ratings still depend on the evaluator’s judgment. I therefore treated the critique as a starting point and used peer feedback to learn how other people actually interpreted my redesign.

## Step three: Sketch a solution

My first idea was to replace the infographic with horizontal bar charts. Bar length would make differences visible, while direct labels would preserve the exact percentages.

I initially considered using a common country order across all four pet categories, sorted by dog ownership, with overall averages as reference points. As I developed the sketch, I realized that this would make it harder to identify the leaders for cats, fish, and birds. I shifted toward four independently sorted panels in a 2 × 2 layout.

I built the sketch in a single Tableau worksheet. Each panel represented one pet type, with countries and regions sorted from the highest to the lowest percentage. I used blue to highlight the top three positions, red to highlight the United States, and gray for the remaining observations. Where the United States also belonged to the top three, its red color took priority.

![Tableau sketch showing four independently sorted pet ownership charts](Pet.png)

This sketch narrowed my main question to: **How does the United States compare with the leading countries and regions for each pet type?**

Independent sorting supported that question, although it introduced a tradeoff: the same country would appear in a different position in each panel. Direct country labels helped readers locate individual observations.

## Step four: Test the solution

I shared my sketch with three classmates during an informal classroom discussion. They looked directly at the visualization, asked questions, and suggested changes. I did not conduct a scripted interview or collect timed task results, so the table below summarizes the feedback they actually provided rather than reconstructing answers to a questionnaire.

All three classmates said the overall information was clear and recognized that the visualization emphasized the United States. Their suggestions focused on wording, readability, layout, and emphasis.

### Results

| Participant | Feedback | Changes made |
| --- | --- | --- |
| Classmate A | Reconsider “ranked” in the subtitle because the chart did not display explicit rank numbers. Percentage labels on both the bars and the axes felt redundant. | Changed the subtitle to “Sorted by percentage within each pet type” and removed numerical axis labels while retaining direct percentage labels. |
| Classmate B | The text was too small. The percentage needed a clearer definition: did it refer to people, households, or the number of pets? “Country” would be more accessible than “market” in the title. | Enlarged the text, clarified that the percentages refer to respondents who have each pet type in their household, and changed the title to “Pet ownership across 22 countries and regions.” |
| Classmate C | Place dogs and cats vertically together, and fish and birds vertically together. Make the top-three labels bold. | Arranged dogs above cats in the left column and fish above birds in the right column, and applied bold formatting to the top-three labels. |

### Synthesis

The feedback suggested that the main visual emphasis was working: readers could identify the focus on the United States. The remaining problems concerned how easily they could read and interpret the supporting information.

A recurring lesson was that wording matters as much as chart structure. Replacing “ranked” with “sorted” described the display more precisely, and clarifying the percentage definition reduced ambiguity. Larger text and fewer repeated numerical labels improved readability.

The layout suggestion also gave the four panels a clearer organization. Placing dogs and cats together grouped the two categories with generally higher ownership percentages, while fish and birds formed the second column. Bold labels added emphasis to the leading observations.

## Step five: build the solution

I completed the redesign in a single Tableau worksheet using four horizontal bar-chart panels.

<div class='tableauPlaceholder' id='viz1794361399055' style='position: relative'><noscript><a href='#'><img alt='Pet ownership across 22 countries and regionsPercentage of respondents who have each pet type in their household, 2016.Sorted by percentage within each pet type. ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pe&#47;Pet_17939993738590&#47;FinalRedesign&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Pet_17939993738590&#47;FinalRedesign' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pe&#47;Pet_17939993738590&#47;FinalRedesign&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object>
</div>
<script type='text/javascript'>
  var divElement = document.getElementById('viz1794361399055');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

The final design uses the title **“Pet ownership across 22 countries and regions.”** Its subtitle explains that the values are the percentages of respondents who have each pet type in their household and that the observations are sorted within each pet category.

Each panel uses the same horizontal scale and a zero baseline, allowing bar lengths to remain comparable across pet types. I removed the numerical axis labels because each bar already shows its percentage. Dogs and cats occupy the left column, while fish and birds occupy the right column.

Blue highlights the top three positions, including ties, and red consistently identifies the United States. The U.S. cat label includes “Top 3” because it belongs to both groups. The other U.S. labels do not include that designation. I also enlarged the text and made the top-three labels bold in response to the classroom feedback.

I did not retain the average reference lines considered during sketching. The final design focuses on identifying the leaders and locating the United States within each category.

### What the redesign shows

- **Dogs:** Argentina leads at 66%, followed by Mexico at 64% and Brazil at 58%. The United States is fourth at 50%.
- **Cats:** Russia leads at 57%, followed by France at 41%. The United States is third at 39%.
- **Fish:** China, Turkey, and Belgium lead at 17%, 16%, and 15%, respectively. The United States is at 11%.
- **Birds:** Turkey leads at 20%, while Brazil and Spain are tied at 11%. The United States is at 6%.

These comparisons show that the United States is relatively close to the leaders for dogs and is among the top three for cats, while it sits farther down the displayed ordering for fish and birds.

### Reflection and limitations

The most useful change was moving from a decorative arrangement of percentages to independently sorted bars. This made the leading observations easier to locate while retaining the broader international context. Classroom feedback then helped me refine the language, typography, and panel arrangement.

There are still tradeoffs. Independent sorting makes it harder to follow a country across all four panels, and the pale gray labels may be difficult to read at smaller display sizes. A future revision could increase the contrast of those labels while preserving the emphasis on the United States and the leading observations. I have not conducted a second round of testing on the final version.

The data also require careful interpretation. The source describes a 2016 survey of more than 27,000 internet users aged 15 and older across 22 markets. These figures are historical survey results, not current estimates for every resident or household. Respondents could report multiple pet types, so the percentages should not be expected to sum to 100%. They describe the presence of a pet type in the household, not the number of animals owned.

The working dataset used for this redesign records Hong Kong’s bird ownership at 5%, whereas the original infographic displays 3%. This discrepancy remains in the final chart.

Overall, this process taught me that a redesign involves more than selecting a different chart type. It also requires deciding which comparisons matter, defining the metric clearly, and checking whether readers notice the intended emphasis.

## References

- NielsenIQ. (2016). [Man’s best friend: Global pet ownership and feeding trends](https://nielseniq.com/global/en/insights/report/2016/mans-best-friend-global-pet-ownership-and-feeding-trends/). Includes the GfK pet ownership infographic and survey information.
- Few, S. [Data Visualization Effectiveness Profile](https://www.perceptualedge.com/articles/visual_business_intelligence/data_visualization_effectiveness_profile.pdf).
- [Design and Redesign](https://medium.com/@hint_fm/design-and-redesign-4ab77206cf9). Assigned course reading.
- [Tableau Public](https://public.tableau.com/). Tool used to develop the sketch and final visualization.

## AI acknowledgements

I used ChatGPT to help troubleshoot Tableau calculations and formatting and revise this Markdown writeup.

[Back to home page](https://wenjiajian77.github.io/tswd-portfolio/)
