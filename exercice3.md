# Netflix Chaos Engineering

### Concrete Experiments :
Netflix conducts various concrete experiments to test the resilience of its systems and ensure seamless service delivery. 

Here are some of the key experiments:

- **Chaos Kong** simulates the failure of an entire **Amazon EC2 region** to evaluate whether Netflix can effectively reroute user traffic to other regions with minimal disruption (conducted on a monthly basis).
- **Chaos Monkey** shuts down virtual machine instances within the production environment.
- **Failure Injection Testing** involves engineers deliberately introducing errors into the communication between services.

### Experiment Requirements :
The experiments are conducted directly in the **production environment** to simulate real-world conditions. Netflix uses its own tools to manage and monitor these failures. Their reliance on **cloud infrastructure**, specifically Amazon Web Services allows them to conduct these geographically distributed tests effectively.

### Observed Variables :
- **Service availability :** measuring whether users can continue streaming content seamlessly.
- **SPS :** tracks how many videos are started each second serving as an overall health indicator of the system.
- **Latency and CPU Usage:** Identifies performance bottlenecks to maintain optimal system functionality.

### Key Results :
The experiments help improve Netflix fault tolerance without degrading user experience. They reveal that even in complex systems failures can be anticipated and managed allowing for controlled responses to disruptions.

### Is Netflix the Only Company Performing These Experiments?
No, other tech like **Amazon Prime Video, Hulu, Disney+ and Spotify** also use chaos engineering techniques to test the resilience of their systems.

### Application to Other Organizations :

- Banks: Simulate database outages to ensure transaction integrity.
- E-commerce: test scenarios like website downtime during peak shopping hours to assess customer impact.
- Telecommunications: Inject network latency to observe how calls and data services handle degraded conditions.

In these cases, the key system variables to observe would include :
- system response times
- error rates
- service availability
