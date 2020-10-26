# ACE Service

## Parse a text string into ACE outpus as paraphrase1 of the input text phrase

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "paraphrase1" as ACEOutput type for parsing

_Then_ The ACE service should return text with full sentences instead of relative clauses.

## Parse a text string into ACE outpus as paraphrase2 of the input text phrase

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "paraphrase2" as ACEOutput type for parsing

_Then_ The ACE service should return text using relative clauses instead of full sentences.

## Parse a text string into ACE outpus as paraphrase of the input text phrase

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "paraphrase" as ACEOutput type for parsing

_Then_ The ACE service should return string with best-effort combination of paraphrase1 and paraphrase2 output.

## Parse a text string into OWL/SWRL in the Functional-Style Syntax reperesentation (prolog term)

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "owlfss" as ACEOutput type for parsing

_Then_ The ACE service should return output as OWL/SWRL in the Functional-Style Syntax representation as prolog term.

## Parse a text string into OWL/SWRL in the Functional-Style Syntax reperesentation (pretty printed)

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "owlfsspp" as ACEOutput type for parsing

_Then_ The ACE service should return output as OWL/SWRL in the Functional-Style Syntax representation term in pretty format.

## Parse a text string into Output as OWL/SWRL in the RDF/XML representation

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "owlrdf" as ACEOutput type for parsing

_Then_ The ACE service should return output as OWL/SWRL in the RDF/XML representation.

## Parse a text string into Output as OWL/SWRL in the XML representation

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "owlxml" as ACEOutput type for parsing

_Then_ The ACE service should return output as OWL/SWRL in the XML representation.

## Parse a text string into output for RuleML representation of the DRS

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "ruleml" as ACEOutput type for parsing

_Then_ The ACE service should return string with corresponding output in ruleML representation of the DRS.

## Parse a text string into ACE outpus as First Order Logic (fol)

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "fol" as ACEOutput type for parsing

_Then_ The ACE service should return string with corresponding output for predicate logic for the text Phrase based on First Order Logic.

## Parse a text string into First Order Logic of predicate logic of (prenex normal form) of the DRS in Prolog term

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "pnf" as ACEOutput type for parsing

_Then_ The ACE service should return array of tokens as strings.

## Parse a text string into Output TPTP representation of the DRS

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "tptp" as ACEOutput type for parsing

_Then_ The ACE service should return Output TPTP representation of the DRS.

## Parse a text string into tokens as a Prolog list of lists

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "tokens" as ACEOutput type for parsing

_Then_ The ACE service should return Output tokens as a Prolog list of lists.

## Parse a text string into Output as simplified syntax trees as a Prolog list

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "syntax" as ACEOutput type for parsing

_Then_ The ACE service should return string as simplified syntax trees as a Prolog list.

## Parse a text string into Output as simplified syntax trees in pretty-printed form

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "syntaxpp" as ACEOutput type for parsing

_Then_ The ACE service should return string as simplified syntax trees in pretty-printed form.

## Parse a text string into output as plain syntax trees as a Prolog list (for debugging).

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "syntaxd" as ACEOutput type for parsing

_Then_ The ACE service should return string as plain syntax trees as a Prolog list for debugging.

## Parse a text string into Output as plain syntax trees in pretty-printed form (for debugging).

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "syntaxdpp" as ACEOutput type for parsing

_Then_ The ACE service should return string as plain syntax trees in pretty-printed form for debugging.

## Parse a text string into the DRS(Discourse Represetnational Structure) as a Prolog term

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "drs" as ACEOutput type for parsing

_Then_ The ACE service should return string as the DRS as a Prolog term.

## Parse a text string into the DRS in XML.

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "drsxml" as ACEOutput type for parsing

_Then_ The ACE service should return string with DRS in XML.

## Parse a text string into the DRS in pretty-printed form in plain text

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "drspp" as ACEOutput type for parsing

_Then_ The ACE service should return string as the DRS in pretty-printed form in plain text.

## Parse a text string into the DRS in pretty-printed form in HTML

_Given_ I have a valid token for mauna services

_When_ I call the ace.mauna.cloud with the token using the graphql query

_And_ Pass text phrase as doc to parseAce query

_And_ pass boolean guess and solo option "drs" as ACEOutput type for parsing

_Then_ The ACE service should return string as the DRS in pretty-printed form in HTML.
