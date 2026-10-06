---
description: How to quickly setup the application
---

# Quick Start

## follow the steps given below to setup:-

> small steps are always better than standing still.
>
> small progress is always better than no progress.

{% hint style="info" %}
Just take small steps that it
{% endhint %}

{% stepper %}
{% step %}
### installation

install all neccesary libraries required
{% endstep %}

{% step %}
### authentication

authenticate all the apus befoire useing
{% endstep %}

{% step %}
### Port Connection

1. choose and set a port for local host testing&#x20;
2. and also add an alteranet port if first is busy
{% endstep %}

{% step %}
### Api building

Building all the apis&#x20;
{% endstep %}
{% endstepper %}





{% code lineNumbers="true" %}
```mermaid
flowchart LR
    A[User] --> B[Login]
    B --> C{Valid Login?}
    C -->|Yes| D[Dashboard]
    C -->|No| E[Show Error]
    E --> B
    D --> F[Select Service]
    F --> G[Process Request]
    G --> H[(Database)]
    H --> G
    G --> I[Success]

```
{% endcode %}

```mermaid
flowchart TD
    A[Start] --> B[User Request]
    B --> C{Request Type}

    C -->|New User| D[Create Account]
    C -->|Existing User| E[Verify Account]
    C -->|Guest| F[Continue as Guest]

    D --> G[Access System]
    E --> G
    F --> G

    G --> H[Process Request]
    H --> I[(Database)]
    I --> J[Generate Result]
    J --> K[End]

```





