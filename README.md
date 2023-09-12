# MagiciansGPT
Can GPT read minds? Think again.

## MagiciansGPT is intended for making GPT a magician's assistant for predicting numbers, card, position of a card, dice roll, and more.
The method is essentially a way of coding information to GPT via prompts in front of the audience.

## Here is an example performance:
Magician: Have you guys heard of ChatGPT? It is basically this crazy smart AI from OpenAI that knows everything and all the tech companies are sprinting catch up. I thought to myself... if it is so powerful, maybe it can read human minds! Let's try an experiment shall we?
\nAudience: Sure!
Magician: Can I borrow your phone and let's go to this link: [magiciansgpt.streamlit.app](magiciansgpt.streamlit.app)
Audience: I see the page now. There is a chatbox.
Magician: Ok now think of a number between 1-10. But don't say it out loud so the mighty AI can't hear it. Oh block the camera on your phone too. Now just use your fingers to let everyone know what number you are thinking.
Audience put up two fingers with victory sign ✌️
Magician: Ok now put it down. Let's ask GPT.
Magician enters the following prompt and then return phone to Audience: "My friend Anne here is thinking of a number. Now tell us what is she thinking."
GPT: 
Audience enters
GPT: 
Audience enters
GPT:
Audience: What?! How does it know?

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

## Dice Roll
This is largely the same as number. Except there are 6 sides to a dice so the possiblities are 1-6. Coding the same as before.
The activation is "think of a dice roll" or "thinking of a dice roll"
The interesting idea here is that magician can force a dice roll with some magicial products such as _Winner's Dice by Secret Factory_. This way the prompt could be made to GPT before the actual roll with prompt like this "My friend is going to think of a dice roll. Think you can predict the outcome?" That will be a 6 on the roll.
Another idea is to use _Mental Die by Tony Anverdi_ so the audience can roll the dice in secret and magician never saw the actual dice roll and yet can input prompt correctly.

## Finger


## Card


## Card Story



### Errors handling

### Credit
Dan Harlan invented an easy version of coding numbers to magician's assistant in front of audience in his DVD - SpeakEasy back in 2011. This is a modernized version with GPT and extended to far beyond just numbers and added other methods of magic in the mix to create the ultimate "Magician's GPT"

License from me is required to use this app in commerical applications or large performances. All rights reserved.


