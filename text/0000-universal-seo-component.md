- Start Date: (fill me in with today's date, YYYY-MM-DD)
- RFC PR: (leave this empty)
- Gatsby Issue: (leave this empty)

# Summary

A universal SEO component that can work on any use cases.

# Basic example

```jsx
// page is an article
<SEO
  type="article"
  
/>
```

# Motivation

One of the things that I enjoyed about Gatsby is the implementation of optimized
images without having to code a ton of things. Similarly, implementing SEO is the same. 
Creating simple projects such as blogs, would only require a couple lines of code and [this](https://www.gatsbyjs.org/docs/add-seo-component/) 
would suffice. However, bigger projects such as e-commerce would require a structured 
data of the product, review, 

# Detailed design

This is the bulk of the RFC. Explain the design in enough detail for somebody
familiar with Gatsby to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

# Drawbacks

Why should we *not* do this? Please consider:

Being a universal components, there's a ton of structured data that we have to account for.
There are <strong>598 Types, 862 Properties, and 114 Enumeration values</strong> in total. That number alone 
should tell us that we shouldn't do this. This would probably set the record for the longest switch statement
in the history of javascript.



- implementation cost, both in term of code size and complexity
- whether the proposed feature can be implemented in user space
- the impact on teaching people Gatsby
- integration of this feature with other existing and planned features
- cost of migrating existing Gatsby applications (is it a breaking change?)

There are tradeoffs to choosing any path. Attempt to identify them here.

# Alternatives

What other designs have been considered? What is the impact of not doing this?

1. Popular use cases only
This mi
# Adoption strategy

If we implement this proposal, how will existing Gatsby developers adopt it? Is
this a breaking change? Can we write a codemod? Should we coordinate with
other projects or libraries?

# How we teach this

What names and terminology work best for these concepts and why? How is this
idea best presented? As a continuation of existing Gatsby patterns?

Would the acceptance of this proposal mean the Gatsby documentation must be
re-organized or altered? Does it change how Gatsby is taught to new developers
at any level?

How should this feature be taught to existing Gatsby developers?

# Unresolved questions

Optional, but suggested for first drafts. What parts of the design are still
TBD?
