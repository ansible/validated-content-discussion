---
name: 'New Validated Content Candidate '
about: Create a discussion issue for a new validated content candidate
title: 'candidate: $NAME'
labels: candidate
assignees: ''

---

#### Candidate Name
<!--example.validated_collection -->


#### Link to Github Repo
<!---link -->

#### CHECKLIST

##### Business Checks:

**Content Viability** 
- [ ] must support a “business-viable” use case
- [ ] isn’t just a demo
- [ ] is production-ready, as in able to run in Ansible Controller “as-is”
- [ ] provides a solution an end-to-end automation use case and brings value to our customers

**Content Duplication**
- [ ] use case addressed by the content isn’t covered by another validated content collection already - to the best of our knowledge

##### Technical Checks:

**Content Conformity**
- [ ] is packaged as a content collection - see the [Collection Requirements Checklist](https://github.com/ansible-collections/overview/blob/main/collection_checklist.md)
- [ ] is YAML only (Exception: if plugin(s) included are necessary for this specific use-case and are not generic enough for a certified collection)
- [ ] if there is a plugin(s), it is not a duplicate of something from a certified or supported collection - to the best of our knowledge
- [ ] supported plugin/module used in a validated role is noted as a dependency

**Content Compliance** 
- [ ] no known policy or legal reason for why the content shouldn’t be published
- [ ] README contains information about the purpose of the collection and how to install it
- [ ] README contains a link to the collection license file
- [ ] README contains general usage and requirements information such as required versions of ansible-core and Python, and other required libraries or SDKs
- [ ] Repo is self-certified with the [OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/en) and has the OpenSSF Best Practices Badge 
- [ ] Has 2 or more active maintainers listed in a CODEOWNERS file. 
- [ ] Has an approved OSI license 
- [ ] Content falls logically into one of these domains - infra, security, network, cloud, edge
- [ ] (If internal content) Content has been or is being migrated into the redhat-cop Github org


**Content Testing/Validation**
- [ ] runs `ansible-lint` “Production” profile in an active Github workflow on the repository
- [ ] passes the `ansible-lint` “Production” profile
- [ ] ansible-lint.yml file (if present) only contains justified ignores - with a comment explaining the need for each ignore
