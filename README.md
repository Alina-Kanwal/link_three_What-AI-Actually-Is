# link_three_What-AI-Actually-Is
Isliye course kehta hai: AI ka confident hona is baat ka saboot nahi ke jawab sahi hai. Jahan topic rare ho, ya jawab ka asar bara ho, wahan aap ko khud check karna hai.
Exam mein yeh aise aayega: scenario mein AI ne kisi chhoti ya anokhi cheez ke baare mein bohat mufassal aur confident jawab diya, to sahi qadam hai ke source se verify karo, na ke jawab maan lo.
Aakhri ek line: AI ek writer hai jo sab se mumkin text likhti hai, librarian nahi jo fact dhoondhti hai.
**Prediction:** AI andaza lagati hai ke agla text kaunsa hona chahiye, jo sunne mein sab se mumkin lage.
**Lookup:** koi kitab ya database khol kar asli fact dhoondna aur wahan se parhna.
**Mashhoor fact:** woh baat jo lakhon baar likhi gayi ho (jaise Pakistan ka founder), isliye AI ka andaza aksar theek nikalta hai.
**Rare fact:** woh baat jo bohat kam likhi gayi ho (jaise aap ke shehar ki chhoti academy ki fees), isliye AI ka andaza ghalat ho sakta hai magar phir bhi confident lagta hai.
**Aap ka nichor lagbhag sahi hai.** Do chhoti correctionein:
1. **"Rata hua" nahi, pattern.** AI jawab yaad nahi karti jaise hum ratte hain. Woh text ke andar ke patterns seekhti hai, aur har baar jawab **naye sire se predict** karti hai. Isliye aksar same sawal par thora alag jawab aata hai.
2. **Hallucination ki wajah Idea 3 mein hai.** Idea 1 sirf yeh batata hai ke AI predict karti hai. "Jawab na pata ho tab bhi bol deti hai" ki asal wajah (andar koi truth-checker nahi) Idea 3 mein aati hai.
**Aap ne jo cover kiya:** AI librarian nahi, aur log use librarian samajhte hain.
**Idea 1 mein aur kya tha (jo aap ke nichor mein nahi aaya):**
1. **Autocomplete ki tasveer:** AI wohi kaam karti hai jo phone "Happy birthday to" ke baad "you" suggest karke karta hai, bas bohat zyada parhi hui hai. Farq: phone aap ke type kiye phrases yaad rakhta hai, AI koi phrase store nahi karti, sirf **numbers** (weights) jo score dete hain ke agla token kaunsa hoga.
2. **Tokens:** AI text ko chhote tukron mein parhti aur likhti hai, aur har naya tukra pichle sab ko dekh kar chunti hai.
3. **Stochastic (spread se chunna):** AI ek nahi, mumkin tokens ki poori list score ke saath nikalti hai aur usmein se ek chunti hai. Isliye same sawal ka jawab har baar thora alag hota hai. **Temperature** dial hai: kam = steady aur dohrata hua, zyada = alag-alag magar kabhi ghalat.
4. **Prediction aur lookup kab ek jaise lagte hain:** mashhoor facts par dono ka jawab ek nikalta hai, isliye farq nazar nahi aata. Rare topic par farq saaf dikhta hai.
5. **"Lekin ChatGPT web search karta hai!":** product karta hai, model nahi. Product ek **tool** lagata hai jo facts laata hai, woh **context window** mein aate hain, aur model phir bhi unhein predict karke hi jawab banata hai (Idea 8).
6. **AI kam "mujhe nahi pata" kehti hai:** kyunke prediction ka kaam hamesha koi agla token dena hota hai. Jab tak usay "nahi pata" kehna trained na kiya gaya ho, woh bol deti hai.
**Exam ke liye sab se zaroori:** AI predict karti hai look up nahi (Idea 1), isliye rare topic par confident jawab aaye to source se verify karo.
Ab "aage" likhein to Idea 2 shuru karta hoon.
