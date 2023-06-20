# Cloud Development Basics

## Security by design

Declares security should be present throughout every step of the process. 

Various models exist to help, like the **Building Security in Maturity Model (BSIMM).** (Pairs well with DevSecOps)

## Shared Security Responsibility 

The idea is that security is the responsibility of everyone from the most junior member of the team ot senior management.(Describes the primary principle of DevSecOps)

## Security as a Business Objective

Risk mitigation through security controls should be a key business objective, similar to customer satisfaction or revenue. (Requires org-wide security awareness and commitment)

# Common Pitfalls

Common pitfalls of application security in the cloud

- Performance
- Scalability
- Interoperability
- Portability
- API Security

## Performance

Cloud software development often relies on lossley coupled services. 

Makes designing for and meeting performance goals more complex, as multiple componenets may interact in unexpected ways. (verify through end-to-end load and stress testing)

## Scalability

One of the key features of the cloud is the ability to scale allowing applications and services to grow and shrink as demand fluctuates.

Requires developers to think about how to retain state across instances and handle faults with individual servers. (Scale out is better than scale up in the cloud)

## interoperability

Is the ability to work across platforms, services, or systems and can be very important, especially multi-vendor and multi-cloud scenarios. (interoperability across platforms increases service provider choice and can reduce costs)

## Portability

Designing software that can move between on premises and cloud environments or between cloud providers makes it portable.

Portability in a hybrid scenario requires avoiding use of certain environment and provider-specific API tools. (The additional effort can make it harder to leverage some cloud advantages and may require compromises)

## API Security

Application programming interfaces (APIs), are relied on throughout cloud application design, development, and operation.

Designing APIs to work well with cloud architectures while remaining secure are both common challenges for developers and architects.

**API Security Considerations:**
- Access Control
- Data Encryption
- Throttling
- Rate limiting

(CSPs offer PaaS services that simplify addressing these concerns, may also address the need to present the API in multiple geographies)