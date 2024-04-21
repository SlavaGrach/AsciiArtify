## Introduction
AsciiArtify is a startup dedicated to creating a new software product that uses Machine Learning to transform images into ASCII art. Founded by two young entrepreneurs who are experienced software developers but lack DevOps expertise, the team faced challenges in selecting a technical solution for developing a local Kubernetes cluster. They evaluated three tools: minikube, kind, and k3d.

## Characteristics
| Characteristics            | Minikube                  | Kind                      | K3d                       |
|----------------------------|---------------------------|---------------------------|---------------------------|
| OS                         | Windows, macOS, Linux     | Windows, macOS, Linux     | Windows, macOS, Linux     |
| Architectures              | x86-64, ARM               | x86-64, ARM               | x86-64, ARM               |
| Automation                 | Yes, via CLI and Helm     | Yes, via CLI              | Yes, via CLI and Helm     |
| Cluster Monitoring         | Yes, via Dashboard        | Yes, via CLI              | Yes, via CLI              |
| Deployment Speed           | Medium                    | High                      | High                      |
| Documentation              | Sufficient                | Good                      | Good                      |
| Community Support          | Extensive                 | Extensive                 | Extensive                 |
| Customization Difficulty   | Medium                    | Low                       | Low                       |
| Docker Alternative (Podman)| Yes                       | Yes                       | Yes                       |

## Advantages and Disadvantages
| Tool      | Advantages                                         | Disadvantages                                      |
|-----------|----------------------------------------------------|----------------------------------------------------|
| Minikube  | Comprehensive tool with built-in monitoring        | Slower deployment, higher resource requirement     |
| Kind      | Fast deployment, integrates well with CI pipelines | Limited to container-based operations              |
| K3d       | Efficient resource usage, fast setup               | May have compatibility issues with certain setups  |

##Demo
[![asciicast](https://asciinema.org/a/655540.svg)](https://asciinema.org/a/655540)

## Conclusion

According to our practical evaluation, k3d is the most suitable tool for AsciiArtify's PoC due to its quick cluster setup and user-friendly interface, making it ideal for initial development. Nevertheless, it should be emphesized that there is limited community documentation and scalability challenges may arise. Additionally, considering potential licensing concerns with Docker, it's advisable for AsciiArtify to explore using Podman instead. AsciiArtify should carefully assess the trade-offs before reaching a final decision.



