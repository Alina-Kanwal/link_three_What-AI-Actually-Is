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
///////////////////////////////////////////////////////////////////////////AI ne ek baar parha, phir seekhna band ho gaya
Aap ki baat sahi pakri hai, yeh bohat ahem hai. Isay ek student ki misal se samjhata hoon.
**Ek student ki misal**
**Marhala 1: Pretraining (bohat saari kitabein parhna)**
Student ne hazaron kitabein, akhbar aur websites parhi hain. Usay yeh aata hai ke **text ke baad agla text kya aata hai.** Usay yeh nahi sikhaya gaya ke koi sawal pooche to jawab dena hai.
Is liye agar aap likhein "Pakistan ka capital kya hai?", to woh isay **agli line ki tarah** continue karta hai, yani "Pakistan ka sab se bara shehar kaunsa hai?" Woh jawab nahi dhoondta, woh text ka agla hissa likhta hai, kyunke exam papers mein sawal ke baad aksar doosra sawal hota hai.
**Marhala 2: Instruction tuning (jawab dena sikhana)**
Ab ek ustad usay **chhoti list** dikhata hai: sawal aur uska theek jawab. Student seekhta hai: *"Jab koi sawal puche to jawab do. Jab koi kaam de to wo kaam poora karo."* Ab model assistant ki tarah jawab dene lagta hai.
**Marhala 3: Style tuning (RLHF, andaaz sudharna)**
Ab kai log student ke alag alag jawab parhkar number dete hain. Jo jawab saaf, madadgaar, aur confident hote hain unhein zyada number milte hain. Student us andaaz ko pasand karna seekh jata hai. **Is ka ek nuksan hai:** yeh confident aur agreeable andaaz sach hone ki guarantee nahi (Idea 6).
**Yaad rakhne ka tareeqa:** *Parho → Jawab dena seekho → Andaaz sudharo.*
**Teeno marhale freeze se pehle hote hain.** Training khatam hote hi weights freeze ho jate hain, aur aap jab model istemal karti hain (**inference**) to un mein kuch nahi badalta.
**Exam mein is par kaun se sawal aa sakte hain (mere andaze se):**
1. **Marhale ka naam:** "Kaun sa marhala model ko sikhata hai ke sawal ka jawab dena hai?" → **Instruction tuning.**
2. **Kya kisi marhale mein seekhna ab bhi chalta hai?** "Aap ne AI ko correction di, kya woh seekh gayi?" → **Nahi.** Model frozen hai, sirf is chat mein madad karti hai.
3. **Confidence ki wajah:** "AI itni confident kyun lagti hai?" → **Marhala 3** (insani ratings confident andaaz ko behtar maante hain), aur sach ki guarantee nahi.
4. **Cutoff:** "AI ko aaj ki khabar kyun nahi pata?" → **Knowledge cutoff**, training ki text ek tay tareekh par ruk gayi.
5. **Memory ka sawal:** "AI agle chat mein purani baat kaise yaad rakhti hai?" → **Model nahi, product ek note save karke har chat ke shuru mein dikhata hai.**
Yeh sawal mere khud ke andaze par hain, official exam ke nahi.
**Ek aakhri line:** pehle marhale mein AI likhna seekhti hai, doosre mein jawab dena, teesre mein andaaz.
"Aage" likhein to Part 2 (tokens) shuru karta hoon, ya "quiz" likhein to Part 1 par English mein sawal.
Encyclopedia ek bari kitab (ya kitabon ka set) hai jis mein duniya ke hazaron topics par mukhtasar maloomat likhi hoti hai, jaise ek hi jagah par tareekh, science, shehron aur mashhoor logon ke baare mein.
Misal: Wikipedia ek online encyclopedia hai. Urdu mein ise “daira-tul-ma’arif” bhi kehte hain.
**Frozen model: poori baat points mein**
- Training khatam hote hi model ke **weights freeze** ho jate hain, aur seekhne ka marhala wahin khatam.
- ChatGPT aur Claude jo aap istemal karti hain, **dono frozen hain**.
- Aap ne chat mein model ko correct kiya, to correction **is chat ke text** mein aa jati hai.
- Model agla jawab usi text ko dekh kar likhta hai, isliye **is chat mein** jawab theek hone lagta hai.
- **Naya chat** kholein to correction wahan nahi hoti, kyunke model ke andar kuch badla hi nahi tha.
- Model tab badalta hai jab **company khud nayi training** karke naya version (nayi weights) release karti hai.
- Is naye version mein **aap ki chat ka koi hissa nahi** hota
//////////////////////////////////////////////////////////////////**Idea 3: AI ke andar sach check karne wala koi hissa nahi hai**
- Ek insaani expert ke andar **do salahiyatein** hoti hain: jawab banana, aur us jawab ko check karna ("kya mujhe pakka yaqeen hai? Yeh maine kahan seekha?"). Yeh dono aapas mein asehmat bhi ho sakti hain.
- AI ke paas **sirf pehli salahiyat** hai (jawab banana). Uske andar koi alag hissa nahi jo jawab bhejne se pehle check kare ke yeh sach hai ya nahi.
- Ek hi process sahi continuation bhi banata hai aur ghalat bhi, aur dono ke beech koi flag nahi hota. Isliye jawab hamesha fluent aur confident aata hai.
- **Hallucination** ka matlab hai ek **fluent, confident, magar jhoota** jumla.
- Yeh koi glitch ya kharabi nahi hai. Machine bilkul waise kaam kar rahi hai jaise banayi gayi hai: jahan sab se mumkin text sach nahi hota, wahan bhi wohi predict karti hai.
- Hallucination ki formula: **rare topic + jawab dene ki majboori + koi checker nahi = confident invention.**
- Tools aur checks upar se lagane se hallucination **kam** hoti hai, magar machine ke andar ki bunyadi cheez nahi badalti.
- Isliye AI ke **confidence par bharosa nahi** kiya ja sakta. Ek banawati statistic usi pur-yaqeen awaaz mein aati hai jis mein asli aati hai (Idea 6 mein is ki wajah aayegi).
**Course ki misal:**
- Ek walid ne AI se apne shehar ki ek chhoti tuition academy ki fees aur timings poochhe, jiski koi website nahi thi.
- AI ne saaf-suthri table di, magar **har figure invent kiya hua tha**.
- Academy training text mein itni kam thi ke predict karne ko koi asli schedule tha hi nahi, to AI ne wohi bana diya jo aisi academy ke liye sab se mumkin lagta.
- Uske paas koi doosri salahiyat nahi thi jo kehti "tum andaza laga rahi ho." **Woh awaaz aap se aani hai.**
**Yaad rakhne ki ek line:** AI ke andar ek hi salahiyat hai (jawab banana), check karne wali doosri salahiyat **aap** hain.
**Exam tip:** rare ya chhoti cheez par AI ne mufassal confident jawab diya aur source nahi diya, to source kholo aur verify karo.



















