<!--
author:    Hannes Tegelbeckers
email:     hannes.tegelbeckers@ovgu.de
version:   0.2.0
language:  en
narrator:  UK English Female
mode:      Presentation
classroom: enable

title:     AI in TVET and Employment Promotion – Applying AI Sensibly
comment:   Virtual inspirational keynote for the GIZ TVET and Labour Market community (12–15 min). Based on V3, with the interlude "A new way to talk to computers".
-->

# AI in TVET and Employment Promotion

**Applying AI sensibly**

**Hannes Tegelbeckers**  
Otto von Guericke University Magdeburg – Engineering pedagogy and technical education

Keynote · GIZ conference of the TVET and Labour Market community

                --{{0}}--
Good morning, everyone, and welcome. I am Hannes Tegelbeckers from Otto von Guericke University Magdeburg, where I work on how people learn technical work. In the next fifteen minutes I want to share a practical view: what should we, the TVET and labour market community, do with AI – and what can we leave to others?

# Setting the scene

AI is already here. The question is how we use it.

                --{{0}}--
Let us start with something we all share. AI is already part of our working and learning lives. For us, the question is not how to build AI – it is how to use it well for real problems.

## AI arrives quietly

                --{{0}}--
Think about your week so far. Most of you have used AI already – probably without calling it AI.

{{1}}
- Spell-check and translation on your phone
- Voice messages turned into text
- Chatbots answering customer questions
- Route planning for delivery drivers
- CVs sorted by recruitment platforms

                --{{1}}--
Imagine Amina, a young job-seeker. Her phone corrects her spelling and turns her voice messages into text. And when she applies online, a platform may sort her CV before any person reads it. She meets AI every day without noticing.

{{2}}
<section>

**AI, in plain words:** software that has learned patterns from many examples – and uses them to suggest, predict, sort or write.

It does not understand like a person. It can be confidently wrong.

</section>

                --{{2}}--
That is the definition I will use today. And please keep the second line in mind: AI can sound very sure and still be wrong. That will matter in every part of this talk.

## Where have you met AI this week?

- [(1)] In my messages and email
- [(2)] At work or in my project
- [(3)] In learning or teaching
- [(4)] Honestly, I don't know

                --{{0}}--
Before we go on, a quick poll – no right answer, just curiosity. Where have you met AI this week? Please click one option now. If you picked "I don't know", you are in good company – that is exactly how quietly AI arrives.

## Apply, don't build

Building big AI models costs huge amounts of money, data and energy – and only a handful of companies do it.

                --{{0}}--
Here is the frame for the whole talk. Building large AI models from scratch is extremely expensive and is done by a handful of companies. That is not our job – and that is good news.

{{1}}
<section>

Our strength is **applying** existing tools to real problems:

- matching people to jobs
- making training more relevant
- supporting teachers

</section>

                --{{1}}--
Our strength lies somewhere else: using tools that already exist, for problems we know well. Matching Amina to a job. Making a training course fit what employers really need. Giving a busy teacher some help.

{{2}}
> We do not need to build the engine – we need to train good drivers and build good roads.

                --{{2}}--
This is my image for today. The engine already exists. Our work is the drivers – skilled people – and the roads – good data, good institutions, good training.

# A new way to talk to computers

From clicking, to coding, to simply saying what you need.

                --{{0}}--
Before the three pillars, one short interlude. Something fundamental has changed in how people work with computers – and it matters a lot for TVET.

## Click → Code → Prompt

Same task: *"Which apprentices missed more than 3 days this month?"*

                --{{0}}--
Look at one everyday task in three ways.

{{1}}
<section>

**🖱️ Click** – open the spreadsheet → Data → Filter → month = October → pivot table → sort → filter > 3

<small>You need to know **where** everything is.</small>

</section>

                --{{1}}--
With clicks, you need to know where every menu is.

{{2}}
<section>

**⌨️ Code**

```python
df = pd.read_excel("attendance.xlsx")
october = df[df.date.dt.month == 10]
n = october[october.absent].groupby("name").size()
print(n[n > 3])
```

<small>Precise and repeatable – but you need to learn a **programming language**.</small>

</section>

                --{{2}}--
With code, you need to learn a programming language.

{{3}}
<section>

**💬 Prompt**

> "Here is our attendance list. Which apprentices missed more than three days in October? Make a short table I can send to the training company."

<small>Your **own words** – any language. Behind the scenes, the AI may write the code above for you.</small>

</section>

                --{{3}}--
With a prompt, you just say what you need – in your own words, maybe even in your own language. Behind the scenes, the AI may write exactly that code for you.

{{4}}
**Why this is empowering:** plain language becomes the interface. A trainer, a technician or a labour-market analyst can **describe** what they need – without being a programmer. But you still have to **know your trade** to judge whether the answer is right.

                --{{4}}--
That is empowering: the barrier to using a computer drops dramatically. But the knowledge of the trade becomes more important, not less – because someone has to judge whether the answer is right.

## Offline or online AI – where does your data go?

                --{{0}}--
Here is a choice every GIZ project will face: offline AI on a server you own, or online AI from a cloud provider.

{{1}}
```ascii
  OFFLINE                                    ONLINE
  +- your institution / your country -+
  |                                    |     +-------------+                          +------------------+
  |  +--------+        +------------+  |     |   laptop    |  ---- internet ----->    | cloud data centre|
  |  | laptop | -----> | local AI   |  |     | prompt+data |                          | abroad,          |
  |  +--------+        | server     |  |     +-------------+                          | commercial       |
  |                    | (open      |  |                                              +------------------+
  |                    |  model)    |  |
  |                    +------------+  |
  +------------------------------------+
        data stays inside                          data leaves
```

                --{{1}}--
Offline AI means an open model running on a server you own – at a university, a ministry, a training centre. The data never leaves the building. Online AI means a commercial cloud service – usually stronger and faster, but your data travels to a data centre abroad.

{{2}}
|                 | 🏫 Offline – local server        | ☁️ Online – cloud service      |
| --------------- | ------------------------------- | ------------------------------ |
| Data            | stays in the building           | travels to a provider abroad   |
| Cost            | hardware once, no fees per use  | pay per use (tokens)           |
| Speed & quality | slower, good for first drafts   | fast, strongest models         |
| This keynote    | first draft in 46 min           | first draft in 4 min           |

                --{{2}}--
I tested both on this very keynote. The local server needed 46 minutes for a first draft; the cloud needed four. The best value came from mixing: draft offline, polish online – with about 64 percent fewer cloud tokens than doing everything in the cloud.

{{3}}
<small>The full comparison: [behind the scenes – one keynote built three ways](https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/behind-the-scenes.html)</small>

## The AI never touches the computer

A language model only **writes text** – sometimes that text is code or a command. A program around it, with permissions **you** set, decides what is actually done.

                --{{0}}--
This is the most important technical idea of the talk, and it is simple. The AI itself never touches a computer. A language model only produces text.

{{1}}
```ascii
+-----------+  task, rules  +----------------+  "write_file …"  +----------------+  allowed?  +------------+
|  Human    | ------------> | Language model | ---------------> | Agent program  | ---------> |  Computer  |
| sets the  |               | only writes    |                  | checks         |            | files,     |
| rules     | <------------ | text / code    | <--------------- | permissions    | <--------- | code, web  |
+-----------+   asks if     +----------------+   result as text +----------------+   result   +------------+
                unsure
```

                --{{1}}--
When that text is a command – "read this file", "write that file" – a separate program, the agent, checks whether it is allowed and only then runs it on the computer. The result goes back to the model as new text.

{{2}}
<section>

How this keynote was drafted offline – from the real log:

| Step | Language model writes                         | Agent program                          |
| ---- | --------------------------------------------- | -------------------------------------- |
| 1    | `read_file inputs/rahmen.md`                  | reading in the project: allowed ✅      |
| 7    | `write_file materials/01-giz-keynote/README.md` | writing in `materials/`: allowed ✅   |
| 20   | `write_file agent_report.md`                  | allowed ✅                              |
| 23   | "All self-checks pass"                        | – done after 47 min                    |

</section>

                --{{2}}--
Here is how this keynote was drafted on our university server: twenty-three steps, each one a piece of text from the model, each one checked and carried out by the agent program.

{{3}}
<section>

**Your decision:** the model now writes `delete inputs/` – "clean up old files". Deleting is not in the permissions. What should happen?

- [( )] The files are deleted – the AI decided it
- [(X)] The agent program blocks it or asks a human – nothing changes until a person allows it
- [( )] The language model deletes the files itself
**************************************************************************
The model can only *write* the command. The agent program checks it against the permissions and stops. If a human clicks "allow", the files are gone – the model "meant well", but the **permission** was the human's decision.
**************************************************************************

</section>

                --{{3}}--
And now you decide: the model asks for something outside the rules. The program stops and asks a human. That is where control lives: in permissions, in sandboxes, in human approval – things we can teach, regulate and own.

# Where does our labour market data come from?

<small>Pillar 1 · Data for labour market analysis</small>

                --{{0}}--
First pillar. If we want better information about jobs and skills, we have to start with a simple question: where does the data actually come from – and who is in it?

## From job ad to decision

Labour market information travels a path – from collecting to deciding.

                --{{0}}--
Labour market information does not fall from the sky. It travels a path, step by step, from the first job ad to a decision in a ministry or a training centre. Some people call this the value chain – I will simply call it the path.

{{1}}
```ascii
collect  →  clean & link  →  analyse  →  share & use
(job ads,    (remove          (trends,     (career guidance,
 surveys,     duplicates,      skill        curriculum updates,
 registers)   map to skills)   gaps)        policy)
```

                --{{1}}--
First we collect: job ads, surveys, registers. Then we clean the data and link it to a common list of skills. Then we look for trends and gaps – and finally people use it for career advice, new curricula and policy.

{{2}}
<section>

AI can help along the way:

- read thousands of job ads a day and pull out the skills
- show what employers ask for **this month**
- suggest jobs to job-seekers – and training for skill gaps

</section>

                --{{2}}--
A real example: the EU agency Cedefop uses this to analyse millions of online job ads and track which skills are in demand in Europe; shared skill lists like ESCO make jobs and skills comparable. The big gain is freshness – what employers need now, not what the last census said. For Amina, this could mean a job suggestion that fits her skills, or a short course that closes her gap.

## Whose data is it?

Job-portal data often sits with private platforms abroad.

                --{{0}}--
Now a harder question: who owns all this data? Very often, job-portal data sits with private companies in other countries – not with the people who need it for decisions.

{{1}}
**Data sovereignty:** our partners keep access to their data – and own it.

                --{{1}}--
Data sovereignty simply means this: ministries, public employment services and TVET authorities keep access to their data and own it. This is not a detail. It is the foundation.

{{2}}
<section>

- **Consent:** people agree – and data is used only for what they agreed to
- **Bias:** a system that learned from past hiring can repeat past discrimination
- **EU AI Act (2024):** AI for hiring, for access to training and for assessing learners counts as **high-risk**

</section>

                --{{2}}--
Job-seekers' personal data needs their consent, protection, and use only for the purpose they agreed to. A system that learned from past hiring can repeat old unfairness, for example against women or minorities. The EU now treats AI in hiring and in education as high-risk, with extra safeguards – a useful reference point for our partners.

{{3}}
One option: run open AI models on **local servers** – the data never leaves the country.

                --{{3}}--
And there is a practical way to keep control: run openly available AI models on your own servers. My own university does exactly this, with a desktop-sized AI server for teaching material.

## The informal sector – the blind spot

Imagine a plumber in Nairobi: skilled, busy, trusted by the neighbours. No CV online. No LinkedIn profile.

                --{{0}}--
Imagine a plumber in Nairobi. Skilled, always busy, trusted by the whole neighbourhood. But you will not find this person on LinkedIn or on any job portal.

{{1}}
<section>

About **2 billion** workers – roughly **6 in 10** worldwide – work informally. In Africa: around **85 %**. <!-- PRÜFEN: latest ILO figures -->

Online job ads show only the formal, urban, digital part.

</section>

                --{{1}}--
And this plumber is not the exception. According to the ILO, about two billion people – roughly six in ten workers worldwide – work informally, and in Africa it is around eighty-five percent. Data from online job ads shows only the formal, urban, digital part of the labour market.

{{2}}
<section>

Ways to make them visible:

- short phone or SMS surveys
- voice skill profiles in local languages
- data from trade associations and informal apprenticeships
- records of skills learned on the job

</section>

                --{{2}}--
So how do we make these workers visible? Short surveys by phone or SMS. Skill profiles recorded by voice, in local languages. Data from trade associations and informal apprenticeships, records that recognise skills learned on the job – and, with consent, data from mobile money or markets.

{{3}}
> If it is not in the data, it is not in the decision.

                --{{3}}--
This is the sentence I want you to keep from this pillar. AI makes this gap bigger – unless we deliberately collect data from the informal sector.

# How should TVET prepare technicians for machines that contain AI?

<small>Pillar 2 · Training *for* AI-supported systems</small>

                --{{0}}--
Second pillar. More and more technical systems in our partner countries contain AI: sensors plus software that spot problems and predict failures. So the question is: how does TVET prepare the people who run and repair them?

## Three systems, one pattern

The AI suggests. The human decides.

                --{{0}}--
Let us look at three examples. They are illustrations, but they show one clear pattern: the AI suggests, the human decides.

{{1}}
| Example                 | The AI says …                   | The technician …                         |
| ----------------------- | ------------------------------- | ---------------------------------------- |
| Smart water network     | "Leak here – this pipe may fail" | checks: is the alarm real?               |
| Solar power             | "This inverter is underperforming" | checks, cleans or replaces parts       |
| Automated production    | "This part looks faulty"        | adjusts settings, keeps camera and light set up correctly |

                --{{1}}--
Imagine Grace, a water technician. Sensors in the pipes report a leak, the software predicts which pipe will fail, and Grace gets a work order on her phone. But only Grace can go and judge whether the alarm is real. The same happens with a solar inverter that underperforms, or a camera that spots faulty parts on a production line.

## What changes for skilled workers

Skilled workers now work **with** the system.

                --{{0}}--
For Grace and her colleagues, the daily work changes. They do not work instead of the system – they work with it.

{{1}}
- Read its suggestions: does this make sense?
- Notice when it is wrong
- Feed it good data, look after the sensors
- Write down problems and report them to the right person

                --{{1}}--
They read what the system suggests and ask: does this make sense? They notice when it is wrong. They keep the sensors and the data in good shape, and they know when to pass a problem on to someone else.

{{2}}
| Level                    | What it means                                         |
| ------------------------ | ----------------------------------------------------- |
| 1. Use                   | operate AI-supported tools safely                     |
| 2. Understand and check  | know what it can and cannot do, spot errors, protect data |
| 3. Maintain and adapt    | keep sensors accurate, update data, find and fix faults |

                --{{2}}--
Here is a simple model with three levels: using the tools, understanding and checking them, and maintaining and adapting them. Every occupation needs its own mix of the three.

{{3}}
<section>

Built into each trade – water technician, electrician, mechatronics technician.

**Not** a separate IT course.

</section>

                --{{3}}--
The key point: these skills belong inside each occupation's training, not in a separate computer course. UNESCO published AI competency frameworks for students and for teachers in 2024 – a good reference to start the conversation. In practice this means: update occupational standards and curricula, train teachers and in-company trainers first, offer realistic equipment or simulations, and work with companies that already run such systems.

# How can AI make learning personal, self-paced and open?

<small>Pillar 3 · Training humans *with* AI</small>

                --{{0}}--
Third pillar. Now we turn the question around. Not training for AI – but how AI can help us train people.

## Learning that fits the learner

Imagine Joseph, an apprentice electrician, learning on his phone in the evening.

                --{{0}}--
Imagine Joseph, an apprentice electrician. During the day he works; in the evening he learns on his phone. What can AI do for him?

{{1}}
<section>

An AI tutor can explain it again:

- in simpler words
- in another language
- with another example

… and give practice questions with instant feedback.

</section>

                --{{1}}--
An AI tutor can explain a topic again – in simpler words, in his own language, with an example from his trade. It can create practice questions and give him feedback right away, at his own pace.

{{2}}
**Open Educational Resources (OER):** free learning materials that anyone may reuse and adapt. AI makes adapting them to a local language or trade much faster.

                --{{2}}--
Open Educational Resources are free, openly licensed materials that anyone may reuse and change. UNESCO adopted a Recommendation on them in 2019. With AI, adapting such material to a local language or a specific trade becomes much faster.

{{3}}
Example from my work: an open-source **Teaching Agent** turns a teacher's course plan into interactive online material. The teacher stays the author. <!-- PRÜFEN: decide whether to mention that this keynote was drafted with it in three ways (offline on a local university server, with a commercial AI assistant, offline first plus human-guided improvement) -->

                --{{3}}--
An example from my own work: an open-source Teaching Agent helps teachers turn their course plan into interactive online material that runs in any browser. The agent drafts, checks and suggests – but the teacher stays the author and decides.

## AI as co-pilot, not autopilot

> AI is a co-pilot – not an autopilot.

                --{{0}}--
Imagine Sara, a teacher at a vocational school. AI can save her time – but it cannot do her job. My rule is simple: AI is a co-pilot, not an autopilot.

{{1}}
| Teachers keep             | Learners need                                 |
| ------------------------- | --------------------------------------------- |
| setting goals             | critical thinking: "Is this correct? How do I check?" |
| judging quality           | problem solving                               |
| relationship, motivation  | communication and teamwork                    |
| fair assessment           | responsibility                                |

                --{{1}}--
Sara keeps what matters most: setting goals, judging quality, motivating her learners and assessing them fairly. And her learners need skills that AI cannot replace – above all, asking: is this answer correct, and how do I check it?

{{2}}
**Risks:** confident wrong answers · copying instead of learning · unequal access · privacy of young learners

                --{{2}}--
Let us name the risks honestly: answers that sound right but are wrong, copying instead of learning, unequal access, and the protection of minors' data. None of these is a reason to stop – they are reasons to teach carefully.

{{3}}
> If teachers are not confident with AI, learners will not be either.

                --{{3}}--
That is why I would start with teachers like Sara. If TVET teachers feel confident with AI, their learners will follow.

# Where should GIZ invest?

                --{{0}}--
Let us bring it together. Where should GIZ projects put their energy? Here are five directions, all drawn from what we have just seen.

{{1}}
- **Low-barrier, mobile-first:** simple phones, messaging, SMS, voice, local languages
- **People before platforms:** teachers, trainers, analysts, employment services
- **Local ownership:** partners own their data; open source, open formats
- **Include the informal sector** – in data and in training
- **Start small, learn fast:** pilots, then scale what works

                --{{1}}--
Solutions that work on a simple phone, with weak internet, by voice and in local languages – and skilled people before new platforms. Partners who own their data and use open tools, so they do not depend on one company – with the plumber in Nairobi included. And small pilots on clear problems – then scale what works and share it across projects.

## Three take-aways

                --{{0}}--
If you remember only three things from this talk, let them be these.

{{1}}
**1. Apply, don't build** – AI is a tool for real problems.

                --{{1}}--
First: apply, don't build. We do not need our own engine. We need to use existing tools for real problems – like getting Amina into the right job.

{{2}}
**2. People first** – skilled workers and teachers who can work with AI and question it.

                --{{2}}--
Second: people first. Technicians like Grace and teachers like Sara, who can work with AI – and who dare to question it.

{{3}}
**3. Data with care** – local ownership, privacy, and the informal sector in the picture.

                --{{3}}--
Third: data with care. Our partners own their data, people's privacy is protected, and the plumber in Nairobi is in the picture too.

## Your turn: where will you start?

- [(1)] Better labour market data
- [(2)] Updating TVET curricula
- [(3)] Training teachers
- [(4)] Reaching the informal sector

                --{{0}}--
One last poll before I close: where would you start in your own project? There is no wrong answer – pick the one your partners already care about.

{{1}}
**Call to action:** bring one real problem from your project to today's discussions. Name the person it is about – and one small pilot you could start.

                --{{1}}--
Here is my request for this conference. Bring one real problem from your project into the discussions – and name the person it is about: a job-seeker, a technician, a teacher, a learner. Then ask together what small pilot you could start next.

{{2}}
> AI will not replace good TVET – but TVET that uses AI well will shape who benefits from it.

                --{{2}}--
AI will not replace good TVET – but TVET that uses AI well will shape who benefits from it. Thank you for your attention, and I look forward to our discussions.


## Play with it – after the talk

| Tool | What you can try |
| ---- | ---------------- |
| [Job-Futuromat (IAB)](https://job-futuromat.iab.de) | which tasks of your occupation can be automated? (German) |
| [Will Robots Take My Job?](https://willrobotstakemyjob.com) | automation risk estimates for US occupations |
| [Teachable Machine](https://teachablemachine.withgoogle.com) | train your own small AI with your webcam |
| [Quick, Draw!](https://quickdraw.withgoogle.com) | doodle and watch an AI guess – and fail |
| [ESCO](https://esco.ec.europa.eu) | the EU's shared list of skills and occupations |
| [Cedefop Skills-OVATE](https://www.cedefop.europa.eu/en/tools/skills-online-vacancies) | skills demand from millions of online job ads |
| [LM Studio](https://lmstudio.ai) · [Ollama](https://ollama.com) | run an open AI model offline, on your own computer or server |

**Interactive web version** (with leak-detection game, skill finder and agent step-through): https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/

**Behind the scenes** – this keynote built three ways (offline, cloud, combined): https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/behind-the-scenes.html

                --{{0}}--
All links for after the talk. Both the web version and this LiaScript version stay online.
