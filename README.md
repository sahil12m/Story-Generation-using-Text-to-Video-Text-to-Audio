# Generating Story using Text-To-Video and Text-to-Audio synchronization

 The project aims development of a cutting-edge story generation system that leverages state-of-the-art Multi-Modal Natural Language Processing (NLP) models (Text-to-Video and Text-to-Audio) to convert textual prompts into immersive audio-visual narratives. The objectives for this project are mentioned below:
 
 1. Develop a state-of-the-art story generation system by enabling users to input prompts and receive audio-visual stories in response.
 2. Incorporate cutting-edge NLP models for text to-video and text-to-audio synthesis.
 3. Solve the audio-video synchronization problem between the generated outputs.

Sample Story Prompt given by user:
In a small town nestled between rolling hills, lived a young girl named Lily. She had a curious pet named Sparky. One day, while exploring the woods behind her house, Lily stumbled upon a mysterious old map. The map seemed to lead to a hidden treasure. With Sparky by her side, Lily embarked on an adventure, facing challenges and overcoming obstacles along the way, until finally reaching a hidden cave. There, the long-lost treasure awaited their discovery. As they uncovered the treasure, a surprise awaited them—it held a secret that would change Lily's life forever.

Sample Output Story Video for above prompt:



https://github.com/sahil12m/Story-Generation-using-Text-to-Video-Text-to-Audio/assets/64885533/1fcd14c2-b2b4-42cb-9a4a-7a8224f403cf

To ensure synchronicity between audio and video we tried 2 approaches:
1) Semantically segmenting the text prompt that the user gives in to feed into the text-to-video model and correspondingly generate music for that segmented part. Continue this loop till the entire user prompt has been traversed and combine the audio and video files using python scripts.
2) Building a GAN that would be able to discriminate our generated output video is a fake/real compared to the real-video of a story and thus this generated feedback is passed back to both the individual text-to-video and text-to-audio pipelines to update the parameters and try to generate a better output. (Still in research)

For seeing a collection of our results:
https://github.com/sahil12m/Story-Generation-using-Text-to-Video-Text-to-Audio/tree/main/Generated%20Stories

For detailed documentation refer to Documentation in the repo.

Contributors:
<br>
<br>
Sahil Mondal<br>
Arham Chouradiya<br>
Jehil Vora<br>
Pranav Parnerkar<br>
Saad Shaikh
