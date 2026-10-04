# Safe Search Operators Reference

This reference contains safe operator templates for ethical public-source research. Replace placeholders such as `Company Name`, `Topic`, `Domain`, and `Person Name` with the target values needed for the research task.

Do not use these patterns to collect private personal data, discover credentials, locate exposed systems, or bypass access controls.

## General Operators

| Operator | Use |
|---|---|
| `"exact phrase"` | Search for an exact phrase |
| `site:example.com` | Limit results to a domain |
| `filetype:pdf` | Find a file type |
| `intitle:keyword` | Find pages with a word in the title |
| `inurl:keyword` | Find pages with a word in the URL |
| `intext:keyword` | Find pages with a word in the body text |
| `OR` | Search for either term |
| `-term` | Exclude a term |
| `before:YYYY-MM-DD` | Find results before a date when supported |
| `after:YYYY-MM-DD` | Find results after a date when supported |

## Business and Company Research

```text
"Company Name" site:companydomain.com
"Company Name" "about" OR "leadership" OR "team"
"Company Name" "press release" OR news OR announcement
"Company Name" "case study" OR testimonial OR review
"Company Name" "annual report" filetype:pdf
"Company Name" "privacy policy" OR "terms of service"
"Company Name" "locations" OR "service area"
"Company Name" "partnership" OR "customer" OR "client"
```

## Competitor and Market Research

```text
"Company Name" competitors
"Company Name" alternatives
"Company Name" vs "Competitor Name"
"Industry" "market report" filetype:pdf
"Industry" "trends" "2026" filetype:pdf
"Service Category" "pricing" "Company Name"
"Service Category" "case study" "Company Name"
"Company Name" "job posting" OR careers
```

## Public Document Discovery

```text
"Topic" filetype:pdf
"Topic" filetype:ppt OR filetype:pptx
"Topic" "white paper" OR "report" filetype:pdf
"Topic" "guide" OR "manual" filetype:pdf
"Topic" "checklist" filetype:pdf
"Topic" "dataset" OR "data set"
"Topic" site:gov filetype:pdf
"Topic" site:edu filetype:pdf
```

## Government and Regulatory Sources

```text
"Topic" site:gov
"Topic" site:regulations.gov
"Topic" site:ftc.gov OR site:consumerfinance.gov
"Topic" site:nist.gov filetype:pdf
"Topic" site:cisa.gov filetype:pdf
"Company Name" site:sec.gov
"Company Name" "10-K" OR "10-Q" OR "8-K" site:sec.gov
"Topic" "guidance" site:gov filetype:pdf
```

## News, Press, and Media Research

```text
"Company Name" "press release"
"Company Name" "interview" OR "podcast" OR "webinar"
"Person Name" "interview" "Company Name"
"Person Name" "conference" OR "keynote" OR "panel" "Company Name"
"Topic" "podcast" OR "webinar" OR "conference"
"Company Name" "announced" after:2025-01-01
"Company Name" "funding" OR "acquisition" OR "partnership"
```

## Academic and Research Sources

```text
"Topic" site:edu
"Topic" "research paper" filetype:pdf
"Topic" "literature review" filetype:pdf
"Topic" "study" OR "survey" filetype:pdf
"Topic" site:scholar.google.com
"Topic" site:arxiv.org
"Topic" site:nih.gov OR site:pubmed.ncbi.nlm.nih.gov
```

## Technical Documentation

```text
"Product Name" documentation
"Product Name" API documentation
"Product Name" "release notes"
"Product Name" changelog
"Product Name" "getting started"
"Product Name" "developer guide" filetype:pdf
site:docs.vendor.com "Topic"
site:github.com "Product Name" "README"
```

## Professional Public-Profile Context

Use these only for legitimate professional context, such as finding official bios, work history stated by the person, speaking appearances, publications, or public professional profiles. Do not use them to assemble private personal profiles.

```text
"Person Name" "Company Name" bio OR biography
"Person Name" "Company Name" speaker OR panelist OR presenter
"Person Name" "Company Name" interview OR podcast OR webinar
"Person Name" site:linkedin.com/in "Company Name"
"Person Name" site:github.com "Company Name"
"Person Name" "article" OR "publication" "Company Name"
```

## Source Verification and Fact Checking

```text
"Exact Claim Phrase"
"Exact Claim Phrase" -site:source-to-exclude.com
"Claim Topic" site:gov OR site:edu
"Claim Topic" "report" OR "study" filetype:pdf
"Quote Text" "Person Name"
"Statistic" "source" "Topic"
"Company Name" "announced" "Date or Year"
```
