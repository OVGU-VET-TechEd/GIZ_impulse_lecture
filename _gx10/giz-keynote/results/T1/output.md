<!--
author:    Hannes Tegelbeckers
email:     hannes.tegelbeckers@ovgu.de
version:   0.1.0
language:  en
narrator:  UK English Female
mode:      Presentation
classroom: enable

title:     AI in TVET and Employment Promotion – Applying AI Sensibly
comment:   Virtual inspirational keynote for the GIZ TVET and Labour Market community (12–15 min).
-->

# AI in TVET and Employment Promotion

--{{0}}--
Good morning, everyone, and welcome. I am Hannes Tegelbeckers from Otto von Guericke University Magdeburg, where I work in engineering pedagogy and technical education. In the next fifteen minutes I will share a practical view: what should we, the TVET and labour market community, do with AI – and what should we leave to others?

# Setting the scene

--{{0}}--
Let us start with a shared observation: AI is already part of our working and learning lives. For us the question is not building AI – it is applying it to real problems.

## AI arrives quietly

--{{0}}--
Think about your week so far. Most of you have used AI already, probably without thinking about it.

{{1}}
- Spell-check and translation in your phone
- Voice messages turned into text
- Chatbots answering customer questions
- Route planning for delivery drivers
- CV screening in recruitment platforms

--{{1}}--
That is the point: AI is already here, quietly.

{{2}}
> AI = software that has learned patterns from many examples and uses them to suggest, predict, sort or write.

--{{2}}--
One important caveat: it does not understand like a person does. It can be confidently wrong. That will matter in every part of this talk.

## Where have you met AI this week?

--{{0}}--
Before we go on, a quick poll – no right answer, just curiosity. Where have you met AI this week?

- [(1)] In my messages and email
- [(2)] At work or in my project
- [(3)] In learning or teaching
- [(4)] Honestly, I don't know

--{{1}}--
Whatever you picked: if it was none of these, you will still meet AI in this talk – because it is already in our jobs and in our classrooms.

## Apply, don't build

--{{0}}--
Here is the framing for the whole talk. Building large AI models from scratch costs huge amounts of money, data and energy, and it is done by a handful of companies. That is not our job.

{{1}}
Our leverage is in **applying** existing tools sensibly to real problems:

- matching people to jobs
- making training more relevant
- supporting teachers

--{{1}}--
My image for the talk: we do not need to build the engine – we need to train good drivers and build good roads.

# Where does the data for labour market analysis come from?

--{{0}}--
First pillar. If we want better labour market information, the first question is a simple one: where does the data come from?

## The labour market information value chain

--{{0}}--
Let us walk the value chain of labour market information, step by step.

{{1}}
```ascii
collect  →  clean & link  →  analyse  →  share & use
(job ads,    (remove          (trends,     (career guidance,
 surveys,     duplicates,      skill        curriculum updates,
 registers)   map to skills)   gaps)        policy)
```

--{{1}}--
Every step is a place where AI can help – and a place where we can make decisions that matter for our partners.

{{2}}
- AI can read thousands of online job ads per day and pull out job titles and required skills
- Real example: the EU agency Cedefop analyses millions of online job ads to track skill demand in Europe (Skills-OVATE)
- Skill lists such as the European ESCO classification help to compare jobs and skills
- AI can suggest jobs to job-seekers and training offers to people with a skill gap
- Real-time signals: what employers ask for *this month*, not only in the last census

--{{2}}--
The value is speed and freshness: we see what employers need right now, not what the last census told us.

## Data governance and sovereignty

--{{0}}--
Who owns the data? Job-portal data often sits with private platforms abroad. Our partners – ministries, public employment services, TVET authorities – should keep access and ownership. That is what we mean by data sovereignty.

{{1}}
- Personal data of job-seekers needs consent, purpose limitation and security
- Bias risk: a system trained on past hiring can repeat past discrimination, for example against women or minorities
- In the EU AI Act (2024), AI used for recruitment and for access to education and vocational training counts as **high-risk** and needs extra safeguards
- Option: run open AI models on local servers, so data never leaves the country – my own university does this with a desktop-sized AI server

--{{1}}--
The message: local ownership is not a detail. It is the foundation.

## The informal sector – the blind spot

--{{0}}--
Here is the blind spot. In many partner countries, most people work informally.

{{1}}
- ILO estimate: about 2 billion workers worldwide, roughly 6 in 10, are in informal employment; in Africa the share is around 85 % <!-- PRÜFEN: latest ILO figures -->
- These workers rarely appear on LinkedIn or in local job portals
- Data from online job ads therefore shows only the formal, urban, digital part of the labour market

{{2}}
Ideas to make them visible: short phone or SMS surveys, voice-based skill profiles in local languages, data from informal apprenticeship and trade associations, recognition of prior learning records, mobile-money or market data – with consent.

--{{1}}--
The numbers come from the ILO; please verify the latest figures before the talk.

--{{2}}--
And the message I want you to keep: if it is not in the data, it is not in the decision. AI makes this gap bigger unless we deliberately collect data from the informal sector.

# How should TVET prepare technicians for AI-augmented systems?

--{{0}}--
Second pillar. The systems our technicians will work on increasingly contain AI. So the question becomes: how should TVET prepare them?

## Three systems, one pattern

--{{0}}--
Let us look at three concrete systems first. In all three cases, the human decides – the AI only suggests.

{{1}}
Three examples (illustrative):

- **Smart water management:** sensors in pipes detect leaks, software predicts where a pipe will fail, and the technician gets a work order on the phone. The technician must still judge whether the alarm is real.
- **Green tech / solar:** monitoring software flags a solar inverter that underperforms; a technician checks, cleans or replaces parts.
- **Automated production:** a camera with image recognition spots faulty parts; operators adjust settings, maintenance staff keep the camera and lighting calibrated.

--{{1}}--
A water technician in Nairobi checking a leak alarm is exactly this: everyday work, not science fiction.

## What changes for skilled workers

--{{0}}--
Skilled workers no longer work *instead of* the system – they work *with* it.

{{1}}
- Read its suggestions and check their plausibility
- Recognise when the system is wrong
- Feed it good data
- Maintain sensors, document and escalate

{{2}}
A simple skill model:

1. **Use** – operate AI-supported tools safely
2. **Understand and check** – know what the system can and cannot do, spot errors, protect data
3. **Maintain and adapt** – calibrate sensors, update data, troubleshoot, configure

{{3}}
The key point: these AI skills must be **job-specific** and embedded in each occupation's training – water technician, electrician, mechatronics technician – not a separate IT course.

- UNESCO published AI competency frameworks for students and for teachers (2024), stressing a human-centred mindset, ethics, AI techniques and applications, and system design
- For TVET: update occupational standards and curricula, train teachers and in-company trainers first, provide realistic training equipment or simulations, and cooperate with companies that already run such systems

--{{1}}--
This is a shift in daily work, and it is already visible in partner countries.

--{{2}}--
Notice the three levels: using, understanding and checking, and maintaining. Each occupation needs a mix of all three.

--{{3}}--
The UNESCO frameworks are a useful reference point for partners who want to start this conversation.

# How can AI make learning personal, self-paced and open?

--{{0}}--
Third pillar. Now we turn the other way: how can AI help us train people?

## Learning that fits the learner

--{{0}}--
AI tutors can explain a topic again in simpler words, in another language, with another example. They can generate practice questions and give instant feedback.

{{1}}
- Self-paced and interactive: learners can learn on a phone in the evening, with interactive quizzes, simulations and step-by-step tasks
- Open Educational Resources – OER – are free, openly licensed materials that anyone may reuse and adapt; AI makes it much faster to adapt OER to a local context, language or occupation (UNESCO adopted a Recommendation on OER in 2019)
- Example: an open-source "Teaching Agent" helps teachers turn their course plan into interactive online course material. The teacher stays the author and decides; the agent drafts, checks and suggests <!-- PRÜFEN: decide whether to mention that this keynote was drafted with it in three ways -->

--{{1}}--
The point is not to replace the teacher. The point is to make good teaching material reachable for every learner, on a phone, in the evening, in their own language.

## AI as co-pilot, not autopilot

--{{0}}--
My rule: AI is a co-pilot, not an autopilot. The human judgement stays at the centre.

{{1}}
- Teachers keep: setting goals, judging quality, relationship and motivation, assessing fairly
- Learners need: critical thinking – "Is this answer correct? How do I check?" – plus problem solving, communication, teamwork and responsibility
- These socio-emotional skills are exactly what AI cannot replace

{{2}}
And let us name the risks honestly: wrong answers that sound confident, copying instead of learning, unequal access, and data protection of minors.

{{3}}
> If TVET teachers are not confident with AI, learners will not be either. Invest in teachers first – they are the gateway.

--{{1}}--
This is a teaching decision, not a technical one.

--{{2}}--
None of these risks is a reason to stop. They are reasons to teach deliberately.

--{{3}}--
This is true for every partner country, and it is where I would start.

# Where should GIZ invest?

--{{0}}--
Let us bring it together. Where should GIZ projects invest? Here are five directions, all from what we have seen today.

{{1}}
- **Low-barrier and mobile-first:** solutions that work on simple smartphones, via messaging apps or SMS, with voice and local languages, with weak internet
- **Capacity building:** TVET teachers, trainers, labour-market analysts and public employment services – people before platforms
- **Local ownership and data sovereignty:** partners own their data and, where possible, run tools locally; prefer open-source and open formats to avoid lock-in
- **Include the informal sector** in data and training offers
- **Start small, learn fast:** pilots with clear problems, then scale what works; share across projects

--{{1}}--
None of these requires building AI. All of them require judgement, partnership and local ownership.

## Three take-aways

--{{0}}--
If you remember one thing from each pillar, it is this.

{{1}}
1. **Apply, don't build** – AI is a tool for real problems.
2. **People first** – skilled workers and teachers who can work with AI and question it.
3. **Data with care** – local ownership, privacy, and the informal sector in the picture.

--{{1}}--
These three are your elevator pitch for the next meeting with a ministry or a vocational college.

{{2}}
One last poll before I close – where would you start in your own project?

- [(1)] Better labour market data
- [(2)] Updating TVET curricula
- [(3)] Training teachers
- [(4)] Reaching the informal sector

--{{2}}--
There is no wrong answer. My suggestion: pick the one your partners already care about, and start small.

{{3}}
> AI will not replace good TVET – but TVET that uses AI well will shape who benefits from it.

--{{3}}--
Thank you for your attention. I hope you leave inspired for the rest of the conference, and I look forward to the discussions.
