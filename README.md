# MagiciansGPT
Can GPT read minds? Think again.

## MagiciansGPT is intended for making GPT a magician's assistant for predicting numbers, card, position of a card, dice roll, and more.
The method is essentially a way of coding information to GPT via prompts in front of the audience.

## Here is an example performance:
Magician: Have you guys heard of ChatGPT? It is basically this crazy smart AI from OpenAI that knows everything and all the tech companies are sprinting catch up. I thought to myself... if it is so powerful, maybe it can read human minds! Let's try an experiment shall we?  
Audience: Sure!  
Magician: Can I borrow your phone and let's go to this link: [magiciansgpt.streamlit.app](magiciansgpt.streamlit.app)  
Audience: I see the page now. There is a chatbox.  
Magician: Ok now think of a number between 1-10. But don't say it out loud so the mighty AI can't hear it. Oh block the camera on your phone too. Now just use your fingers to let everyone know what number you are thinking.  
Audience put up two fingers with victory sign ✌️  
Magician: Ok now put it down. Let's ask GPT.  
Magician enters the following prompt and then return phone to Audience: "My friend Anne here is thinking of a number. Now tell us what is she thinking."  
GPT: Ah, I see! Anne got a number in mind, huh? 🤔 Alright, before I reveal her number, let me try to tap into her thoughts. 🧠✨  Hmm... I sense that you might have a favorite color. 🌈 Is that true? What is it?  
Audience enters "Red"  
GPT: Hot red, huh? That's an interesting choice! Now, let me dig a little deeper into your mind. 🧐 Hmm... I'm picking up some vibes from you. It seems like you enjoy outdoor activities. 🏞️ Am I right about that?  
Audience enters "Yes!"  
GPT: Ah, I knew it! The great outdoors is your playground! 🌳 Now, let me unlock the secrets hidden within your mind and discover that number you've been thinking of. 🤔 I'm feeling quite confident about this... don't tell me just yet, let me concentrate... 🧘‍♀️ Your number is... drumroll... 0! Am I right? 🎉  
Audience: What?! How does it know?  

The process is **Prompt -> Audience answers questions from GPT -> Reveal**
The above example utilizes the "number" module. There are 5 modules MagiciansGPT as follows.

## Numbers
The coding method is simple. There is an activation phrase and then there is the code.  
Activation is "thinking of a number" or "think of a number". When either of those phrases is in prompt, the app will look for the first letter in the following sentence as well as the final punctuation.  
T - 1  
N - 2  
M - 3  
R - 4  
L - 5  

At the end of the prompt, if there is period (.) or question mark (?), that represents + 5.   
So for example:  
Prompt: "My friend John will think of a number. Let's see if you can read his mind."  
"think of a number" triggered number module and "L" means 5 and the end period means +5. That is total of 10 coded to GPT which will be used in the "mind reading".  
And lastly, if there is only one sentence with single period at the end like "I'm thinking of a number." This will mean the number 0.

## Dice Roll
This is largely the same as number. Except there are 6 sides to a dice so the possiblities are 1-6. Coding the same as before.
The activation is "think of a dice roll" or "thinking of a dice roll"
The interesting idea here is that magician can force a dice roll with some magicial products such as _Winner's Dice by Secret Factory_. This way the prompt could be made to GPT before the actual roll with prompt like this "My friend is going to think of a dice roll. Think you can predict the outcome?" That will be a 6 on the roll.
Another idea is to use _Mental Die by Tony Anverdi_ so the audience can roll the dice in secret and magician never saw the actual dice roll and yet can input prompt correctly.

## Finger
For this module, magician can ask the audience to point up with any finger without saying anything or simply touch one of the finger.  
The activation is "think of a finger" or "thinking of a finger" and the rest is similar to the number module except each letter now represents the finger:  
T - Thumb  
N - Index  
M - Middle  
R - Ring  
L - Pinky  

## Card
This module is recommanded after doing some of the previous modules because in module, the magician will not need to prompt the GPT directly. The method is a force and the card being force is the 9 of diamonds.  
Audience can prompt themselves with something like "I'm thinking of a card", the activation is "think of a card" or "thinking of a card".  
Since this is a force, audience could prompt it first and then during the random question phase, magician force a card to the audience before the GPT reveal. Some simple card forcing techniques are here: [Youtube](https://www.youtube.com/watch?v=sxP-tu10ulM)  

## Card Story
And lastly, this is the finale module and shall be used last. This is essentally asking the GPT to create a story utilizing the card information provided.

First, the card deck will need ot be in the Mnemonica order, a popular card stack by Juan Tamariz. Some details [here](https://ulearnmagic.com/mnemonica-stack-order-juan-tamariz/).  
Maigican can say something like "Imagine each of the 52 cards in the deck is like a person. And each card has a story just like each of us. Why don't you think of a card this time in your mind. Any card at all." While explaining this, casually do false shuffles and cuts on the card deck or with help of audience. Some simple false shuffle techniques are here: [Youtube](https://www.youtube.com/watch?v=PfbOELSTyP0)    
At this point, magician will ask the audience to prompt anything with "story" in it along with the card they are thinking of but do not tell magician the card. Few examples like "Tell me a story with Ten of Spades" or "Write a story about Queen of hearts"  

This will take longer processing due to the langchain in place to generate a story title along with the story itself and an image generation prompt to illustrate the story scene (To be implemented at later date)  

While this is happening, magician can explain that "All story happens at a place, a location, or an address. And in the world of a playing card, the address indicates the position of the card in the deck. Now you could have named any card and you never told me what it is. We have a shufflede deck here. Let's see what GPT says."  
GPT: "The Ace of Diamonds Miracle"  
"Once upon a time a young girl named Snow was walking down 39th Street in search of a way to make her dreams come true. She was feeling hopeless and lost, until something strange caught her eye. It was a shining Ace of Diamonds that lay on the sidewalk near her feet. She couldn’t believe her luck and quickly scooped it up. As she peered closer, she saw a slight glimmer of magic coming off of the card. Snow smiled and knew she was exactly where she was supposed to be. She held the card close to her heart, and a miracle occurred. Suddenly all of her dreams seemed within reach and she had hope that everything was going to work out. 🤩🤩✨💎"  

In the story generated, an address will be found along with the card. That will be the same position of the card named in the deck that has been seemingly shuffled and the most amazing part is that magician never knew the card until the story has been generated.

### Errors handling
At rare cases where magician prompted incorrectly that is not following the framework, GPT will respond with:  
"I'm sorry my psychic energy just had a blip.😵‍💫 Could you say that again?🥺"  
"I don't think that card exists in the standard 52 card deck. Try again.🥺"  
This means invalid entry and please prompt correctly again.


### Credit
Dan Harlan invented an easy version of coding numbers to magician's assistant in front of audience in his DVD - SpeakEasy back in 2011. This is a modernized version with GPT and extended to far beyond just numbers and added other methods of magic in the mix to create the ultimate "Magician's GPT"

***License from me is required to use this app in commerical applications or large performances/TV specials. All rights reserved. If you are also Magician+Dev combo, Let's collab!***


