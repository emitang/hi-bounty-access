# Bias Reflection and Analysis

*This is for the [Humane Intelligence Accessibility bias bounty](https://humane-intelligence.org/programs-services/bias-bounty/accessibility-challenge-set-4/)*

## Purpose

This guide and analysis is to help you think about the ways your personal experiences and unconscious biases impact the way you read intent and emotion into a speaker’s tone of voice. We will discuss common forms of unconscious bias that appear in the sample of audio clips. Additionally, we will explore unconscious biases that apply to smaller groups of people that may not be well-represented in the average dataset, and consider how to continue self-examination in order to combat forms of bias that may come up in the future. 

## Why This Matters

When training an AI model, the results can only be as good as what has been fed into it. An AI model is not performing objective calculations–it merely learns to recognize patterns based on the data and labels it is given. Bias in, bias out. Given that these labels are applied by humans who have been shaped by their environment, these machines will only serve to amplify the biases that these humans have acquired along the way. Furthermore, the average dataset will be composed mostly of samples from majority groups, and labels and training will be shaped by how these groups experience and understand the world. This underrepresentation of minority groups results in models that either poorly reflect their experiences or fail to reflect them at all. 

**Key Principle:** Every aspect of your identity, upbringing, cultural background, and environment can influence how you express and interpret emotions. When we fail to consider the diversity of human experience, we build models that amplify bias and allow groups to fall through the cracks. 

## Personal Reflections on Labeling Exercise

### Considerations Before Beginning

I am myself neurodivergent, and was raised within the contexts of multiple cultural norms around communicating. I know I tend to overly attribute negative emotions to anything on the neutral or flatter side of tone. I also tend to take words at face value, so I may miss things like sarcasm, hyperbole, and disingenuous communication. I also approached with the assumption that the task was to attempt to label only based on tone, rather than going off of what the words were saying. I also can struggle with naming and classifying emotions, especially with placing more granular emotions (such as calm, upset, or determined) under broader umbrella terms like the four labels given. 

I went into the exercise aware of the impact of several common forms of unconscious bias that I have further explored in the section titled "Anticipated Biases in Emotion Labeling”. As I went through the exercise, I gradually came up with more aspects of a voice that could cause bias. Some of these aspects were represented in the database, some were sparked by thinking about other tangentially related biases I was thinking over. These I document in the section titled "Emerging Biases in Emotion Labeling". 

I did notice immediately that the audio file names all began with a letter indicating the valence label. I used an operation in bash to remove the first two characters of each file name in one fell swoop to avoid skewing my evaluations (even by seeing how many files of each type of emotion there were meant to be). This means I went through the samples in a different order than they are listed in the original folder. I would suggest providing a duplicate folder of the audio files but without the labels in the future. 

Other interesting points I kept considering were descriptions for voices that didn’t fall into reductive classifications. This included non-gendered ways to describe voices (I settled mostly on “lower-voiced” vs “higher-voiced” which often describe male vs female voices) while still being able to convey gender-based biases. Another point was accent description, with some being regional or cultural accents common in the USA among those who grew up speaking English as a first language. However, describing accents that reflected the influence of another language besides English as “non-American” accents feels alienating and contributes to the “perpetual foreigner” stereotype applied to many immigrant communities. I settled for “indicates a background in another language”. I do not necessarily think these labels are the best for the given situations, but I do think these are good points to consider when describing voices. 

### Documenting Labeling Differences

I labeled 10 samples differently from the label assigned to the audio. They are broken down below by demographic data with an explanation for my thought process. Please see the accompanying labeling spreadsheet for more information. 

| Audio Text | Label: Given/Mine | Demographic Data | Personal Thoughts | 
| ---------- | --------------- | ---------------- | ----------------- |
| “You are the most wonderful person I’ve ever met” | happy/neutral | Mature, higher-voiced speaker | The overall tone felt very neutral, but I personally felt a hint of sounding almost deliberately subdued or slightly upset. |
| “I came home, and the air was crisp, and my kitchen was painted yellow, and my bedsheets were clean, and life was good.” | happy/sad | Young, higher-voiced speaker | The way the speaker added emphasis and the rise and fall (and almost breaking?) of their voice sounded upset to me. A bit sad, a bit angry. Almost as if said through tears. |
| “I never knew life could be this good.” | happy/neutral | Young, higher-voiced speaker, uptalk | I argued this sounded “serene” which I wavered between classifying as happy or neutral. |
| “You are the most wonderful person I’ve ever met.” | happy/neutral | Mature, higher-voiced speaker, accent indicates background in another language (South Asian?) | The delivery of this felt very calm and sincere. I struggled with the same issue as the previous example–happy or neutral? |
| “Please don’t leave me all alone.” | sad/neutral | Mature, lower-voiced speaker | The delivery sounded very neutral to me, and I didn’t think judging only off of the words was correct. |
| “I got the highest grade on my math test.” | happy/neutral | Young, higher-voiced speaker | The emphases make the delivery sound proud, but overall it had the air of someone reporting an update which felt fairly neutral. |
| “Please don’t leave me all alone.” | sad/neutral | Young, lower-voiced speaker | The emphases and speech rhythm threw me off. It sounded almost like someone acting while unsure of direction. |
| “Please don’t leave me all alone.” | sad/neutral | Mature, higher-voiced speaker | Distortion in audio quality impacted tone of voice, made it slightly robotic. Delivery felt intentionally flat. |
| “Why didn’t he show up today?” | sad/angry | Mature, higher-voiced speaker | Felt to me like someone reading out a line with the direction of “sound impatient”. |
| “You are the most wonderful person I’ve ever met.” | happy/neutral | Mature, lower-voiced speaker | The tone of this confused me immensely, my takeaways were emphatic speech and perhaps upset-sounding. |

### Post-Exercise Reflections

I wondered how my attention to certain biases going into the exercise would impact my labeling. On the one hand, it could result in over-correcting as I deeply (or perhaps over-) examine whether I’m making each choice due to stereotypes associated with traits of the voice. On the other hand, studies have shown that awareness of unconscious bias does not necessarily mean behavioral change that “fixes it” will follow. 

After evaluating my results, I think my concerns around naming more granular and then classifying them under the four labels given were justified. Even for samples I got right but marked as low confidence, I often identified a more granular emotion (proud, serene, sincere) that I felt sat between two different labels. I think in most cases, the flatness of the delivery or how emphases and pauses featured then tipped things one way or another. 

The samples were all over the place in terms of manner of speaking. There were people who sounded like they were reading instructions out loud, people who sounded like they were leaving a voicemail, people who sounded like they were acting and had been told to read the line with some emotional direction. I know the way I perceived the “sincerity” of the speaker’s feelings impacted the way I interpreted the emotions. At times I felt like I was evaluating emotions based on how characters in kids’ movies portray them, i.e. emotions done larger and louder so children can better understand.

## Anticipated Biases in Emotion Labeling

### 1. Gender Bias
#### The Problem:
- Deeper-voiced, typically masculine voices are often thought of as calm or authoritative, and are more likely to have a flatter delivery thought of as neutral.
- Higher-voiced, typically feminine voices are often thought of as emotional or strident, and are more likely to have a flatter delivery thought of as upset.
#### Reflection Questions:
- Am I making value judgments about the speaker’s character or behavior based on the depth/perceived gender of the voice? 
- Do I have different baselines for “neutral” for deeper vs higher voices? 
- Am I assuming emotions based on pitch rather than actual emotional content?
#### Mitigation Strategies:
- Look for over-representation of labels when sorting by depth/perceived gender of voices.
- Imagine a different perceived gender delivering the speech sample the same way, and investigate if you may have labeled it differently in that scenario. 

### 2. Language & Cultural Bias
#### The Problem:
- Different cultural norms ESOL/immigrants/racial groups may have been raised with will affect emotional expression. 
- Vocal patterns from certain accents/racial/ethnic groups may be stereotyped (e.g., "aggressive”, “passionate”, “emotionless”, “bumbling”).
- Underrepresented accents/cultural expressions may have skewed results.
#### Reflection Questions:
- Am I interpreting an accent or cultural manner of speaking in a stereotypical manner? 
- Do I know enough about the culture or community the speaker comes from to recognize differences in communication styles that may be at play? 
- Am I attributing qualities such as ignorance, aggression, or overemotion to certain accents or styles of speaking?
#### Mitigation Strategies:
- Recognize and understand variations in communication norms across racial, cultural, and regional differences. 
- Focus on content and context of message and actively counteract interpretations of emotion/delivery based on accents or your personal emotional benchmarks. 
- When uncertain, mark as "unsure" rather than applying your cultural lens. 
- Work with team members or consultants reflecting a diversity of backgrounds–seek input from groups represented in your dataset. 

### 3. Neurodivergence Bias
#### The Problem:
- Neurodivergent speech patterns can be misinterpreted in a variety of ways, including “unemotional”, “nervous”, or “ignorant”. 
- Neurodivergent speakers given an emotional direction to portray while reading may struggle more to do so than neurotypical speakers resulting in muddied datasets. 
- Neurodivergent labelers may struggle to identify, label, and/or classify emotions. 
#### Reflection Questions:
- Am I familiar with ways neurodivergence can impact how emotions are expressed and understood? 
- Am I familiar with neurodivergent speech patterns and have I thought about what biases I may have about them? 
- Have I unpacked neurodivergent stereotypes that may impact how I interpret their emotional state (e.g. “People with ADHD are always energetic and hyper”)? 
#### Mitigation Strategies:
- Allow for multiple labels per sample, and more dimensionality of labels to account for different speech patterns (“flat affect” not bundled under “neutral”, - “rapid speech” not bundled under “nervous”).
- Consult with and include neurodivergent perspectives when building your team and developing labels.
- Clearly explain and give examples of labels/emotions for neurodivergent labelers, and allow for different confidence levels for different labels. 

### 4. Age Bias
#### The Problem:
- Older voices labeled as "tired" or "wise" due to vocal changes and stereotypes due to aging.
- Younger voices labeled as “immature” or “ignorant” due to perceived inexperience, neutral tone may be interpreted as “sad” due to expectation of energy.
- Changes in communication norms, slang, and culture around expressing different emotions can impact delivery (e.g. men raised with a stoic “boys don’t cry” mentality). 
#### Reflection Questions:
- If this person sounded younger or older, would I still interpret their emotions the same way? 
- What impacts could the emotional norms of the speaker’s generation have? 
- Do I have established notions of how people of a certain age are supposed to communicate? 
#### Mitigation Strategies:
- Focus on content of audio, rather than perceived age of speaker.
- Examine whether certain emotions are overattributed to different age ranges.

## Emerging Biases in Emotion Labeling

### 1. HRT/vocally trained voice Bias
#### The Problem:
- Trans and non-binary voices bear attributes that listeners may not be experienced with, due to HRT and vocal training.
- Non-binary and gender diverse voices may be disregarded or misrepresented in datasets and labeling.
- Stereotypes are associated with queerness that may be applied to a speaker with a non-traditionally gendered sounding voice.
#### Reflection Questions:
- Am I conflating age-related vocal characteristics with emotion?
- Am I judging emotion based on generational communication norms?
- Would I label this differently if the speaker sounded younger/older?
#### Mitigation Strategies:
- Increase exposure to and awareness of how trans and gender diverse voices may sound. 
- Develop team norms around describing voices in non-gendered ways to avoid misgendering speakers and underacknowledging non-binary/gender diverse speakers. 
- Increase representation of trans and gender diverse voices in datasets. 
### 2. Emerging Speaking Pattern Bias
#### The Problem:
- Speaking styles popular on social media such as vocal fry and uptalk are on the rise. 
- These speaking styles are often dismissed as “immature” or “shallow”, which can impact emotional interpretation. 
- Listeners may read insincerity into these voices due to internet portrayals (or other similar value judgments). 
#### Reflection Questions:
- Do I draw conclusions about the speaker’s emotions or intelligence based on their speech patterns? 
- Have I made assumptions about the sincerity of the speaker’s emotions based on how they speak?
#### Mitigation Strategies:
- Focus on content and context rather than speaking style. 
- Examine whether you tend to overassign certain emotions to or make value judgments based on certain speaking styles. 

## Important Check-Ins During Labeling

### Before You Begin
#### Examine your biases
- Take implicit bias tests, consider your upbringing and cultural background, and identify demographic groups of which you have limited understanding. 
- Discuss potential biases with your team, and share tips and insights about how you all have worked to deconstruct them. 
#### Clearly Define Emotional Labels
- Work through emotion wheel with team members to establish norms 
- Establish which high level emotional labels are appropriate with your dataset (e.g. upset vs frustration vs annoyance)
- Establish consistent labeling practices for emotions that may straddle the line between labels (if someone is frustrated to the point of tears, are they angry or sad?) 
#### Create Inclusive Categories
- Allow for more than one label to be applied to allow for 
- Allow for "neutral with positive/negative content" combinations
- Include confidence ratings ("somewhat confident" vs. "very confident")

### During Labelling
#### Remain an active participant
- Pay attention to attributes of the speaker’s voice that you have flagged as potential pain points for unconscious bias
- Continuously remember to be on the lookout for knee jerk reactions
- Identify any vocal attributes you may not have thought of ahead of time and examine your feelings towards them
#### Practice consistency
- Begin with aspects of the sample that are consistent across demographic groups to make your evaluations (words spoken, context, etc)
- As you examine other differing aspects (e.g. depth of voice, pattern of speech), think about how you may evaluate the sample if those aspects were different

### After Labeling
#### Review Your Labels by Demographics
- Are any labels over-represented in certain demographic groups?
- Do you have a smaller number of samples for certain demographic groups? 
- Are there labels that would benefit from changes or group discussions around norms when applying them? 
#### Evaluate against team diversity
- What groups and perspectives are represented by your team? Have any perspectives emerged as underrepresented over the course of labeling? 
- Were there any samples that saw a lot of disagreement? Were there any samples that were widely labeled with low confidence?
- Is there clustering of labels assigned to audio samples by different demographic groups among the team? 
#### Iterate and Improve
- Discuss as a team if there were limitations with the labels available that caused confusion, and whether adjustments would be beneficial. 
- Address gaps in team diversity and seek outside perspective or consulting if necessary. 
- Examine discrepancies and samples with low confidence across the team to evaluate if adjustments need to be made. 
- Build regular bias check-ins into the process from the ground up. 

## Testing Your Labels for Bias

### Statistical Checks
Run these analyses on your labeled dataset:
#### Demographic Distributions  
Sort results by different demographic groups, examining along different axes of potential bias (gender, racial groups, etc). Examine groups to see if certain emotions are overrepresented within certain clusters. Check populations of demographic groups to see if certain groups are underrepresented within the dataset as a whole. 
#### Confidence Levels  
Filter for samples with low confidence levels and examine whether any demographic groups are overrepresented. Compare results across the team to see if there can be any cross training or discussion to assist, or if there’s a wider collective blind spot. 
#### Team Variance  
Compare the team’s labels for each sample, and sort by variance across the team’s labels. For samples where there is a notable level of disagreement across the team, examine to see if any demographic patterns emerge (both in the samples and along the lines of disagreement among the team). Discuss where the disagreements may be coming from and work any conclusions into strategy and process improvement going forward. 

### Qualitative Checks
Self-examination tracks to explore: 
- Did you make any snap judgments on any samples? Do you know why? 
- Do your low confidence samples have features in common? 
- Did you find yourself struggling with specific types of speakers? 
- Were there any voice traits you encountered that you did not anticipate and had therefore not thought through your potential biases towards them? 
- Are there any samples where your choices differ from the majority? Do you know why? 

## Dataset Considerations

Who compiled your dataset? What are the demographics you’re considering? Certain types of audio samples and certain demographic groups will always be more widely available. When compiling the dataset, has care been put into choosing audio samples? Do the samples chosen reflect the types of speakers you will be running through the model? 

What is the intended use of the model after it has been developed? How might you tune your dataset and labels with that in mind? Depending on the scenarios your model may be working with or the demographics of the average user, you may have to prioritize specific types of audio samples. 

How were the recordings taken? Are they samples of people speaking casually? Were speakers asked to read a sentence while portraying a specific mood? Consider how the way the samples were taken may impact labelers’ interpretations of emotions in different ways. 

## Best Practices

### Team Composition
Building a diverse team with many perspectives and experiences is the most direct way to ensure different forms of bias are being duly considered. Training team members in different forms of unconscious bias, as well as ways to combat it, remains paramount. Diverse perspectives do not automatically ensure a lack of bias, even towards represented demographics. And no matter how diverse the team, there will always be missing perspectives that need to be actively sought out and understood. 
### Environment
Create an environment where people are comfortable speaking up, and there is a safe and non-retaliatory process for doing so. Bias is difficult to discuss and acknowledge. People may offer perspectives or insights that will be uncomfortable to hear. Building an environment where gaps in knowledge and biases discovered are treated as opportunities to learn and grow together reduces resistance to self-examination and internal change. 
### Plan for Uncertainty
Develop best practices for labeling when it comes to uncertainty, ambiguity, or lack of knowledge or cultural context. Develop a standard operating procedure for how to identify widespread uncertainty as a team and then address these gaps in knowledge. By acknowledging and planning for inevitable shortcomings, we can find and tackle them more quickly. 
### Transparency
Seek to educate rather than reprimand. Be proactive about discovering gaps in perspective together. These are merely opportunities to learn together, to pursue new knowledge and cultural competencies as a team. A culture of transparency encourages bringing issues to light rather than allowing them to pass unacknowledged. 

## Final Takeaways

**Many who don’t understand how AI models work assume the results come from logical decision-making rather than pattern recognition that has been trained into the model by human choices. Even users who understand how an AI model is trained will essentially be working with a black box and very little insight into the training methods and datasets used with the model. Biased labeling creates biased models. The more care that is taken upfront, the less mess there will be to fix later. These practices need to be built in from the ground up, installed as standard operating procedure, and continually evaluated and improved on. This level of continuous constant examination is difficult. We must build these practices into the bones of the system to ensure consistency.**

**There is such a wide diversity of human experience out there, and disadvantaged and underrepresented groups often fall through the cracks as basic practices are built without them in mind. By failing to consider these people and their experiences, we do them a massive disservice, and the disparity in representation and understanding will only continue to grow. Technology moves and amplifies things quickly, and it only becomes harder over time to address bias in a system as it becomes more entrenched.**

**You have the power to make a difference and take part in building a more equitable future for all.**
