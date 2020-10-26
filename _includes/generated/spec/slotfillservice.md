# Slot Filling Services

## Entity extraction and slot filling

_Given_ I have a valid token for mauna services

_When_ I call the slot-filling.mauna.cloud with the token using the graphql query

_And_ pass the searchPhrases and phrase to match with the search phrases

_Then_ The slot-filling service should return array of matchPhrases containing words in the phrase that matched with the searchPhrases

_And_ each match word will have the attbutes search_phrase_words, document_word, match_type, similarity_measure, involves_coreference, extracted_word, explanation.
