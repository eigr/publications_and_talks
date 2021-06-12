# TOC

- Serverless on the BEAM with polyglot language support for everyone
- The eigr.io project
- The Protocol
- On the BEAM
- Our Challenges
- eigr/massa
- Demo
- Questions

# 1. Serverless on the BEAM – with polyglot language support for everyone

- develop general purpose applications
- polyglot
    - state management
        - state models (None, EventSourcing, CRUD, CRDTs, ...)
        - inversion of state

> marcel: I think we can explain that the technical basis for such a serverless runtime (can we call it runtime?) and its tech stack, does not mean that we would expect an Elixir/Erlang OTP Developer would choose for to develop distributed applications. But for anyone who likes to develop in Python, JS or any supported language, she can. In this regard, the benefits of the OTP/BEAM runtime helps to enable an environment where the advantages of "serverless" and cloud native can help to be productive.

# 2. The eigr.io project

> marcel: The Idea is to give context. How it started; I think [Jonas' Talk](https://www.youtube.com/watch?v=J3PyYmdTsnQ) at Kubecon was foundational. Then Cloudstate came along with an idea how to implement. There, the CS-Protocol is the most important asset I think. As we state, we build eigr/massa as a Cloudstate compatible proxy. Said, its compatible with Cloudstate, that does not mean it can't do its own stuff, with an enganced protocol. I seriously doubt LB will bring Cloudsdtate on par with Akkaserverless; too much has changed. But, we mihght be surprised.


> marcel: Some thoughts from my usualy context of work. Mostly in fintech here in Switzerland. This for sure does not apply to everything: There is the narrative why we would build a serverless stack, where, serverless today seems to be a product. As LB found out, they can't make a business out of having Cloudstate as an open source project, but have to provide the Serverless experience as a product. For me, having the serverless experience to build "general purpose applications" should be possible, without being locked to a vendor. If my IT can manage kubernetes workload, eigr/serverless, or however we call that, would be on a private or public cloud, I'd control the thing in its entirety. Depending who you ask for, but what I see in my work experience, no serious traditional project would use a serverless product like the one from Lightbend to build their traditional general purpose application in its entirety or any I can think of. For most, it's too risky still at the moment leaning on such a model to build applications. So in this regards our project is an implementation of the ideas Cloudstate established, not being locked in to a vendors product that you can't escape at all without a software escrow option. New businesses building in the open or that are used to use services in the cloud, are comfortable to use serverless services in the cloud.

> marcel: I really think we have to explain why we do this project. Why serverless at all, and why is statemmanagement hard in this area. With the recent beta of akkaserverless, one can find questions and discussions about why the model cloudstate has choosen regarding state is the right one and what problem it solves. FaaS serverless is well understood, but it seems not what cloudstate is doing. Why is it better to bring state to the userfunction, before the userfunction is running at all? I think so far this is not well enough explained and therefore there is no "aha" or "oh yes" effect one would expect to see here. Its interesting to read Lightbends marketing material in this regards; but I would like to have a great explanation by us in our talk, one that shows what actual problem we, and cloudstate, are solving.

# The Protocol

- based on Cloudstate

> marcel: I'd explain the high level stuff. Message-In/Message-Out, the proxy, gRPC, Discovery, Entity-Models, language supports. I'm hesistated to use the term SDK, as AkkaServerless does, we're not a product. But we'll see, dapr.io also has SDKs I think.

# On the BEAM

- why

> marcel: here comes why the BEAM and OTP is a perfect fit for our project as we think. One can say, the OTP/BEAM running the eigr/massa proxy is like a control-plane of a large telephone switch, where user-functions and the messages that go in and out are the data-plane the proxy manages. Sure, the BEAM might be "slow"? for stuff like protocol some will say, we'll see if that is the case.

# Our Challenges

# eigr/massa

- how

# Demo

# Questions
