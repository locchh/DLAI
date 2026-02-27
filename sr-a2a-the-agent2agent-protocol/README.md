## A2A: The Agent2Agent Protocol
 
```ascii
+---------------------------+                    +---------------------------+
|             +----------+  |                    |                           |
|             |  A2A     |  | --Send requests--> |   * Agent URI             |
|             |  Client  |  |   * using the URI  |   * Protocol binding      |
|             +----------+  |   * over supported |                           |
|                           |     binding        |   Agent B                 |
|   Agent A                 |                    |                           |
|                           |                    +---------------------------+
|   Client Agent            |                         | * Agent URI
+---------------------------+                         | * Protocol binding      
                                                 +-----------+
                                                 | Agent     |
                                                 | Card      |
                                                 +-----------+
                                          /.well-known/agent-card.json
```

## Agent Card

`.well-known/agent-card.json`

## Protocol Support
- Json-RPC
- gRPC
- HTTP JSON

## Execution Mode

- **Synchronous**: Waiting for an immediate response
- **Asynchronous**: Proceeding without blocking for a reply
- **Streaming**: Transmitting continous data flows
- **Push Notification**: Alerting the other agent when specific events occur (Wehook & Callback)


## Content Type

Message:
    - Role (user, agent)
    - Parts (text, file or JSON)

Task:
    - ID
    - Current Status

Artifact
    - ID
    - Parts (text, file or JSON)

## Course Repos & Resources

- Course notebooks and scripts: If you'd like to run the notebooks of the next lessons locally, you can find the files and the instructions in this [repo](https://github.com/holtskinner/A2AWalkthrough/tree/main).

- Agent Stack - Healthcare Agent: In lesson 11 (Running A2A Agents on Agent Stack), Sandi will walk you through how to run the agents on BeeAI's Agent Stack using this [repo](https://github.com/sandijean90/AgentStack-HealthcareAgent/tree/main).

- Resources for lesson 2 (A2A architecture):
    - [A2A Documentation](https://a2a-protocol.org/latest/)
    - [this sample app](https://github.com/agntcy/agentic-apps/tree/main/tourist_scheduling_system).

- Resources for lesson 11 (Running A2A Agents on Agent Stack):

    - [Agent Stack documentation](https://agentstack.beeai.dev/stable/introduction/welcome)
    - [More documentation on the Server SDK](https://agentstack.beeai.dev/stable/agent-integration/overview)
    - [Deployment starter example format](https://github.com/i-am-bee/agentstack-starter)
    - [Agent Stack github](https://github.com/i-am-bee/agentstack)

- More A2A agent examples: [A2A Samples](https://github.com/a2aproject/a2a-samples)
