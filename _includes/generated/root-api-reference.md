## API Reference

<details>
  <summary markdown='span'><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [ACEDocument](#acedocument)
    * [ACEResult](#aceresult)
    * [Batch](#batch)
    * [Cat](#cat)
    * [ContextResult](#contextresult)
    * [CorefCluster](#corefcluster)
    * [DialogAlternative](#dialogalternative)
    * [Doc](#doc)
    * [DocExtension](#docextension)
    * [ModelMeta](#modelmeta)
    * [Nlp](#nlp)
    * [ParaphraseResult](#paraphraseresult)
    * [PhraseMatch](#phrasematch)
    * [Query](#query)
    * [SSMLResult](#ssmlresult)
    * [STTResult](#sttresult)
    * [Scores](#scores)
    * [SlingDocument](#slingdocument)
    * [SlingMention](#slingmention)
    * [SlingToken](#slingtoken)
    * [Span](#span)
    * [SpanExtension](#spanextension)
    * [TTSResult](#ttsresult)
    * [TextAlternative](#textalternative)
    * [Token](#token)
    * [TokenExtension](#tokenextension)
    * [WordMatch](#wordmatch)
    * [app_events](#app_events)
    * [apps](#apps)
    * [apps_mutation_response](#apps_mutation_response)
    * [conversation_events](#conversation_events)
    * [conversations](#conversations)
    * [conversations_mutation_response](#conversations_mutation_response)
    * [developer_events](#developer_events)
    * [developers](#developers)
    * [developers_mutation_response](#developers_mutation_response)
    * [end_user_conversations](#end_user_conversations)
    * [end_user_conversations_mutation_response](#end_user_conversations_mutation_response)
    * [history](#history)
    * [kv_store](#kv_store)
    * [last_utterance](#last_utterance)
    * [subscription_root](#subscription_root)
    * [utterances](#utterances)
    * [utterances_mutation_response](#utterances_mutation_response)
  * [Inputs](#inputs)
    * [ContextObject](#contextobject)
    * [DiarizationConfig](#diarizationconfig)
    * [Int_comparison_exp](#int_comparison_exp)
    * [RecognitionMetadata](#recognitionmetadata)
    * [STTConfig](#sttconfig)
    * [SpeechContext](#speechcontext)
    * [String_comparison_exp](#string_comparison_exp)
    * [TTSConfig](#ttsconfig)
    * [app_events_bool_exp](#app_events_bool_exp)
    * [app_events_order_by](#app_events_order_by)
    * [app_status_comparison_exp](#app_status_comparison_exp)
    * [apps_arr_rel_insert_input](#apps_arr_rel_insert_input)
    * [apps_bool_exp](#apps_bool_exp)
    * [apps_insert_input](#apps_insert_input)
    * [apps_obj_rel_insert_input](#apps_obj_rel_insert_input)
    * [apps_on_conflict](#apps_on_conflict)
    * [apps_order_by](#apps_order_by)
    * [apps_set_input](#apps_set_input)
    * [conversation_events_bool_exp](#conversation_events_bool_exp)
    * [conversation_events_order_by](#conversation_events_order_by)
    * [conversations_arr_rel_insert_input](#conversations_arr_rel_insert_input)
    * [conversations_bool_exp](#conversations_bool_exp)
    * [conversations_insert_input](#conversations_insert_input)
    * [conversations_obj_rel_insert_input](#conversations_obj_rel_insert_input)
    * [conversations_on_conflict](#conversations_on_conflict)
    * [conversations_order_by](#conversations_order_by)
    * [conversations_set_input](#conversations_set_input)
    * [developer_events_bool_exp](#developer_events_bool_exp)
    * [developer_events_order_by](#developer_events_order_by)
    * [developers_bool_exp](#developers_bool_exp)
    * [developers_on_conflict](#developers_on_conflict)
    * [developers_order_by](#developers_order_by)
    * [developers_set_input](#developers_set_input)
    * [end_user_conversations_arr_rel_insert_input](#end_user_conversations_arr_rel_insert_input)
    * [end_user_conversations_bool_exp](#end_user_conversations_bool_exp)
    * [end_user_conversations_insert_input](#end_user_conversations_insert_input)
    * [end_user_conversations_obj_rel_insert_input](#end_user_conversations_obj_rel_insert_input)
    * [end_user_conversations_order_by](#end_user_conversations_order_by)
    * [end_user_conversations_pk_columns_input](#end_user_conversations_pk_columns_input)
    * [history_bool_exp](#history_bool_exp)
    * [history_order_by](#history_order_by)
    * [jsonb_comparison_exp](#jsonb_comparison_exp)
    * [kv_store_bool_exp](#kv_store_bool_exp)
    * [kv_store_order_by](#kv_store_order_by)
    * [kv_store_pk_columns_input](#kv_store_pk_columns_input)
    * [last_utterance_bool_exp](#last_utterance_bool_exp)
    * [last_utterance_order_by](#last_utterance_order_by)
    * [ltree_comparison_exp](#ltree_comparison_exp)
    * [money_comparison_exp](#money_comparison_exp)
    * [speaker_type_enum_enum_comparison_exp](#speaker_type_enum_enum_comparison_exp)
    * [timestamptz_comparison_exp](#timestamptz_comparison_exp)
    * [tstzrange_comparison_exp](#tstzrange_comparison_exp)
    * [utterances_arr_rel_insert_input](#utterances_arr_rel_insert_input)
    * [utterances_bool_exp](#utterances_bool_exp)
    * [utterances_insert_input](#utterances_insert_input)
    * [utterances_obj_rel_insert_input](#utterances_obj_rel_insert_input)
    * [utterances_order_by](#utterances_order_by)
    * [utterances_set_input](#utterances_set_input)
  * [Enums](#enums)
    * [ACEOutputType](#aceoutputtype)
    * [AudioEncoding](#audioencoding)
    * [Encoding](#encoding)
    * [InteractionType](#interactiontype)
    * [MicrophoneDistance](#microphonedistance)
    * [OriginalMediaType](#originalmediatype)
    * [RecordingDeviceType](#recordingdevicetype)
    * [app_events_select_column](#app_events_select_column)
    * [apps_constraint](#apps_constraint)
    * [apps_select_column](#apps_select_column)
    * [apps_update_column](#apps_update_column)
    * [conversation_events_select_column](#conversation_events_select_column)
    * [conversations_constraint](#conversations_constraint)
    * [conversations_select_column](#conversations_select_column)
    * [conversations_update_column](#conversations_update_column)
    * [developer_events_select_column](#developer_events_select_column)
    * [developers_constraint](#developers_constraint)
    * [developers_select_column](#developers_select_column)
    * [developers_update_column](#developers_update_column)
    * [end_user_conversations_select_column](#end_user_conversations_select_column)
    * [history_select_column](#history_select_column)
    * [kv_store_select_column](#kv_store_select_column)
    * [last_utterance_select_column](#last_utterance_select_column)
    * [order_by](#order_by)
    * [speaker_type_enum_enum](#speaker_type_enum_enum)
    * [utterances_select_column](#utterances_select_column)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [Float](#float)
    * [ID](#id)
    * [Int](#int)
    * [String](#string)
    * [UUID](#uuid)
    * [app_status](#app_status)
    * [jsonb](#jsonb)
    * [ltree](#ltree)
    * [money](#money)
    * [timestamptz](#timestamptz)
    * [tstzrange](#tstzrange)
  * [Interfaces](#interfaces)
    * [Container](#container)

</details>

### Query (query_root)
query root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_events</strong></td>
<td valign="top">[<a href="#app_events">app_events</a>!]!</td>
<td>

fetch data from the table: "app_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#app_events_select_column">app_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#app_events_order_by">app_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#app_events_bool_exp">app_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

fetch data from the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contextParse</strong></td>
<td valign="top">[<a href="#contextresult">ContextResult</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">turnObjects</td>
<td valign="top">[<a href="#contextobject">ContextObject</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_events</strong></td>
<td valign="top">[<a href="#conversation_events">conversation_events</a>!]!</td>
<td>

fetch data from the table: "conversation_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversation_events_select_column">conversation_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversation_events_order_by">conversation_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversation_events_bool_exp">conversation_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

fetch data from the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_events</strong></td>
<td valign="top">[<a href="#developer_events">developer_events</a>!]!</td>
<td>

fetch data from the table: "developer_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developer_events_select_column">developer_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developer_events_order_by">developer_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developer_events_bool_exp">developer_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

fetch data from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

fetch data from the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

fetch data from the table: "end_user_conversations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">conversation_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">end_user_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>generateSSML</strong></td>
<td valign="top"><a href="#ssmlresult">SSMLResult</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">styledSSML</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">voiceCSS</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history</strong></td>
<td valign="top">[<a href="#history">history</a>!]!</td>
<td>

fetch data from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

fetch data from the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

fetch data from the table: "kv_store" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">key</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope_object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance</strong></td>
<td valign="top">[<a href="#last_utterance">last_utterance</a>!]!</td>
<td>

fetch data from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>matchPhrase</strong></td>
<td valign="top">[<a href="#phrasematch">PhraseMatch</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">analyze_derivational_morphology</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">debug</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">embedding_based_matching_on_root_words</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">ontology_name</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">overall_similarity_threshold</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">perform_coreference_resolution</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">phrase</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">search_phrases</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nlp</strong></td>
<td valign="top"><a href="#nlp">Nlp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">disable</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">model</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>paraphrase</strong></td>
<td valign="top">[<a href="#paraphraseresult">ParaphraseResult</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>parseACE</strong></td>
<td valign="top"><a href="#acedocument">ACEDocument</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">guess</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">solo</td>
<td valign="top"><a href="#aceoutputtype">ACEOutputType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>predictDialogTurn</strong></td>
<td valign="top">[<a href="#dialogalternative">DialogAlternative</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">alternatives</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">history</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speechToText</strong></td>
<td valign="top">[<a href="#sttresult">STTResult</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">audio</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">config</td>
<td valign="top"><a href="#sttconfig">STTConfig</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>textToSpeech</strong></td>
<td valign="top"><a href="#ttsresult">TTSResult</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">config</td>
<td valign="top"><a href="#ttsconfig">TTSConfig</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

fetch data from the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

### Mutation (mutation_root)
mutation root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>delete_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

delete data from the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

delete data from the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

delete data from the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

insert data into the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#apps_insert_input">apps_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_apps_one</strong></td>
<td valign="top"><a href="#apps">apps</a></td>
<td>

insert a single row into the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#apps_insert_input">apps_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

insert data into the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#conversations_insert_input">conversations_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conversations_one</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

insert a single row into the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#conversations_insert_input">conversations_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_mutation_response">end_user_conversations_mutation_response</a></td>
<td>

insert data into the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_user_conversations_one</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

insert a single row into the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

insert data into the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#utterances_insert_input">utterances_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_utterances_one</strong></td>
<td valign="top"><a href="#utterances">utterances</a></td>
<td>

insert a single row into the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#utterances_insert_input">utterances_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

update data of the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#apps_set_input">apps_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

update data of the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#conversations_set_input">conversations_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_developers</strong></td>
<td valign="top"><a href="#developers_mutation_response">developers_mutation_response</a></td>
<td>

update data of the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#developers_set_input">developers_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

update data of the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#utterances_set_input">utterances_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
</tbody>
</table>

### Objects

#### ACEDocument

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>doc</strong></td>
<td valign="top"><a href="#aceresult">ACEResult</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### ACEResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Batch

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>batch_id</strong></td>
<td valign="top"><a href="#uuid">UUID</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>docs</strong></td>
<td valign="top">[<a href="#doc">Doc</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### Cat

Categories applied to whole document (label, score), or to spans (start, end, label, score).

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>label</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

#### ContextResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>document</strong></td>
<td valign="top"><a href="#slingdocument">SlingDocument</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>userId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
</tbody>
</table>

#### CorefCluster

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>i</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

#### DialogAlternative

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>rank</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Doc

A container for accessing linguistic annotations.
Access sentences and named entities.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>cats</strong></td>
<td valign="top">[<a href="#cat">Cat</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The named entities in the document. Returns a list of named entity Span objects, if the entity recognizer has been applied.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#docextension">DocExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noun_chunks</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The base noun phrases in the document.
    Returns a list of base noun-phrase Span objects, if the document has been syntactically parsed.
    A base noun phrase, or “NP chunk”, is a noun phrase that does not permit other NPs to be nested within it – so no NP-level coordination, no prepositional phrases, and no relative clauses.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentiment</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The the sentences in the document.
    Sentence spans have no label. To improve accuracy on informal texts, spaCy calculates sentence boundaries from the syntactic dependency parse.
    If the parser is disabled, the sents iterator will be unavailable.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

The tokens of the document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

#### DocExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contextual_spellCheck</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_nfh</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nfh</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nfh_items</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>outcome_spellCheck</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>performed_spellCheck</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score_spellCheck</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suggestions_spellCheck</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### ModelMeta

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lang</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>license</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pipeline</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sources</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>spacy_version</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Nlp

A text-processing pipeline

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>batch</strong></td>
<td valign="top"><a href="#batch">Batch</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">batch_id</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">batch_size</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">next</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">texts</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>doc</strong></td>
<td valign="top"><a href="#doc">Doc</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>meta</strong></td>
<td valign="top"><a href="#modelmeta">ModelMeta</a></td>
<td></td>
</tr>
</tbody>
</table>

#### ParaphraseResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### PhraseMatch

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>overall_similarity_measure</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>word_matches</strong></td>
<td valign="top">[<a href="#wordmatch">WordMatch</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### Query

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>predictDialogTurn</strong></td>
<td valign="top">[<a href="#dialogalternative">DialogAlternative</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">alternatives</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">history</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### SSMLResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ssml</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### STTResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternatives</strong></td>
<td valign="top">[<a href="#textalternative">TextAlternative</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### Scores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mention</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

#### SlingDocument

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mentions</strong></td>
<td valign="top">[<a href="#slingmention">SlingMention</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#slingtoken">SlingToken</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### SlingMention

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>begin</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>evokes</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>length</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phrase</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### SlingToken

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>size</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>word</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Span

A slice from a Doc object.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conjuncts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#spanextension">SpanExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>label</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lefts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rights</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>root</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentiment</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

A scalar value indicating the positivity or negativity of the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

#### SpanExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coref_cluster</strong></td>
<td valign="top"><a href="#corefcluster">CorefCluster</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coref_scores</strong></td>
<td valign="top">[<a href="#scores">Scores</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>get_has_spellCheck</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_nfh</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_coref</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_nfh</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score_spellCheck</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

#### TTSResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audio</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### TextAlternative

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>transcript</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Token

An individual token — i.e. a word, punctuation symbol, whitespace, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ancestors</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>children</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cluster</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conjuncts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dep</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The ending character offset of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ent_iob</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ent_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#tokenextension">TokenExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>head</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The index of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_alpha</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_ascii</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_bracket</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_currency</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_digit</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_left_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_lower</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_oov</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_quote</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_right_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_sent_start</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_space</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_stop</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_title</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_upper</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lang</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>left_edge</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lefts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_email</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_num</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_url</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lower</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>norm</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>orth</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content (identical to Token.text).
    Exists mostly for consistency with the other attributes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pos</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Coarse-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prob</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>right_edge</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rights</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentiment</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

A scalar value indicating the positivity or negativity of the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shape</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The starting character offset of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suffix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tag</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Fine-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>whitespace</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### TokenExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coref_clusters</strong></td>
<td valign="top">[<a href="#corefcluster">CorefCluster</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>get_require_spellCheck</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>get_suggestion_spellCheck</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>in_coref</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_deter_nfh</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_implicit</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_nfh</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nfh_head</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score_spellCheck</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

#### WordMatch

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>document_phrase</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>document_word</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>explanation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extracted_word</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>involves_coreference</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>match_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>search_phrase_word</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>similarity_measure</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

#### app_events

columns and relationships of "app_events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps">apps</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps

Test this stuff


columns and relationships of "apps"


<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers">developers</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### apps_mutation_response

response of any mutation on the table "apps"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of affected rows by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

data of the affected rows by the mutation

</td>
</tr>
</tbody>
</table>

#### conversation_events

columns and relationships of "conversation_events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations

columns and relationships of "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps">apps</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

#### conversations_mutation_response

response of any mutation on the table "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of affected rows by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

data of the affected rows by the mutation

</td>
</tr>
</tbody>
</table>

#### developer_events

columns and relationships of "developer_events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developers

columns and relationships of "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### developers_mutation_response

response of any mutation on the table "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of affected rows by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

data of the affected rows by the mutation

</td>
</tr>
</tbody>
</table>

#### end_user_conversations

columns and relationships of "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_mutation_response

response of any mutation on the table "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of affected rows by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

data of the affected rows by the mutation

</td>
</tr>
</tbody>
</table>

#### history

columns and relationships of "history"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
</tbody>
</table>

#### kv_store

columns and relationships of "kv_store"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers">developers</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
</tbody>
</table>

#### last_utterance

columns and relationships of "last_utterance"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### subscription_root

subscription root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_events</strong></td>
<td valign="top">[<a href="#app_events">app_events</a>!]!</td>
<td>

fetch data from the table: "app_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#app_events_select_column">app_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#app_events_order_by">app_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#app_events_bool_exp">app_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

fetch data from the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_events</strong></td>
<td valign="top">[<a href="#conversation_events">conversation_events</a>!]!</td>
<td>

fetch data from the table: "conversation_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversation_events_select_column">conversation_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversation_events_order_by">conversation_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversation_events_bool_exp">conversation_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

fetch data from the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_events</strong></td>
<td valign="top">[<a href="#developer_events">developer_events</a>!]!</td>
<td>

fetch data from the table: "developer_events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developer_events_select_column">developer_events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developer_events_order_by">developer_events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developer_events_bool_exp">developer_events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

fetch data from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

fetch data from the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

fetch data from the table: "end_user_conversations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">conversation_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">end_user_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history</strong></td>
<td valign="top">[<a href="#history">history</a>!]!</td>
<td>

fetch data from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

fetch data from the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

fetch data from the table: "kv_store" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">key</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope_object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance</strong></td>
<td valign="top">[<a href="#last_utterance">last_utterance</a>!]!</td>
<td>

fetch data from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

fetch data from the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

#### utterances

columns and relationships of "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_mutation_response

response of any mutation on the table "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of affected rows by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

data of the affected rows by the mutation

</td>
</tr>
</tbody>
</table>

### Inputs

#### ContextObject

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>content</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>userId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td></td>
</tr>
</tbody>
</table>

#### DiarizationConfig

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>enableSpeakerDiarization</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxSpeakerCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minSpeakerCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

#### Int_comparison_exp

expression to compare columns of type Int. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### RecognitionMetadata

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audioTopic</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>industryNaicsCodeOfAudio</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interactionType</strong></td>
<td valign="top"><a href="#interactiontype">InteractionType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>microphoneDistance</strong></td>
<td valign="top"><a href="#microphonedistance">MicrophoneDistance</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>originalMediaType</strong></td>
<td valign="top"><a href="#originalmediatype">OriginalMediaType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>originalMimeType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recordingDeviceName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recordingDeviceType</strong></td>
<td valign="top"><a href="#recordingdevicetype">RecordingDeviceType</a></td>
<td></td>
</tr>
</tbody>
</table>

#### STTConfig

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeLanguageCodes</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audioChannelCount</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>diarizationConfig</strong></td>
<td valign="top"><a href="#diarizationconfig">DiarizationConfig</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enableAutomaticPunctuation</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enableSeparateRecognitionPerChannel</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enableWordConfidence</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enableWordTimeOffsets</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>encoding</strong></td>
<td valign="top"><a href="#encoding">Encoding</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageCode</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxAlternatives</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#recognitionmetadata">RecognitionMetadata</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>model</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>profanityFilter</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sampleRateHertz</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speechContexts</strong></td>
<td valign="top">[<a href="#speechcontext">SpeechContext</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>useEnhanced</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
</tbody>
</table>

#### SpeechContext

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>boost</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phrases</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
</tbody>
</table>

#### String_comparison_exp

expression to compare columns of type String. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_ilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_like</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nlike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nsimilar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_similar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### TTSConfig

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audioEncoding</strong></td>
<td valign="top"><a href="#audioencoding">AudioEncoding</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>effectsProfileId</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pitch</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sampleRateHertz</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speakingRate</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>volumeGainDb</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

#### app_events_bool_exp

Boolean expression to filter rows from the table "app_events". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#app_events_bool_exp">app_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#app_events_bool_exp">app_events_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#app_events_bool_exp">app_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money_comparison_exp">money_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree_comparison_exp">ltree_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange_comparison_exp">tstzrange_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### app_events_order_by

ordering options when selecting data from "app_events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_order_by">apps_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### app_status_comparison_exp

expression to compare columns of type app_status. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#app_status">app_status</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#app_status">app_status</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### apps_arr_rel_insert_input

input type for inserting array relation for remote table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#apps_insert_input">apps_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_bool_exp

Boolean expression to filter rows from the table "apps". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#apps_bool_exp">apps_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#apps_bool_exp">apps_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status_comparison_exp">app_status_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_insert_input

input type for inserting data into table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_arr_rel_insert_input">conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_obj_rel_insert_input

input type for inserting object relation for remote table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#apps_insert_input">apps_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_on_conflict

on conflict condition type for table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#apps_constraint">apps_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#apps_update_column">apps_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_order_by

ordering options when selecting data from "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_order_by">developers_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### apps_set_input

input type for updating data in table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversation_events_bool_exp

Boolean expression to filter rows from the table "conversation_events". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#conversation_events_bool_exp">conversation_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#conversation_events_bool_exp">conversation_events_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#conversation_events_bool_exp">conversation_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money_comparison_exp">money_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree_comparison_exp">ltree_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange_comparison_exp">tstzrange_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversation_events_order_by

ordering options when selecting data from "conversation_events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_arr_rel_insert_input

input type for inserting array relation for remote table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#conversations_insert_input">conversations_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_bool_exp

Boolean expression to filter rows from the table "conversations". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#conversations_bool_exp">conversations_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#conversations_bool_exp">conversations_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_insert_input

input type for inserting data into table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_obj_rel_insert_input">apps_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_arr_rel_insert_input">end_user_conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_arr_rel_insert_input">utterances_arr_rel_insert_input</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_obj_rel_insert_input

input type for inserting object relation for remote table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#conversations_insert_input">conversations_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_on_conflict

on conflict condition type for table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#conversations_constraint">conversations_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#conversations_update_column">conversations_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_order_by

ordering options when selecting data from "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_order_by">apps_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### conversations_set_input

input type for updating data in table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developer_events_bool_exp

Boolean expression to filter rows from the table "developer_events". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#developer_events_bool_exp">developer_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#developer_events_bool_exp">developer_events_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#developer_events_bool_exp">developer_events_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#money_comparison_exp">money_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#ltree_comparison_exp">ltree_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange_comparison_exp">tstzrange_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developer_events_order_by

ordering options when selecting data from "developer_events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data_ron</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_cost</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developers_bool_exp

Boolean expression to filter rows from the table "developers". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#developers_bool_exp">developers_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#developers_bool_exp">developers_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developers_on_conflict

on conflict condition type for table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#developers_constraint">developers_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#developers_update_column">developers_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developers_order_by

ordering options when selecting data from "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### developers_set_input

input type for updating data in table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_arr_rel_insert_input

input type for inserting array relation for remote table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_bool_exp

Boolean expression to filter rows from the table "end_user_conversations". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_insert_input

input type for inserting data into table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_obj_rel_insert_input">conversations_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_obj_rel_insert_input

input type for inserting object relation for remote table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_order_by

ordering options when selecting data from "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### end_user_conversations_pk_columns_input

primary key columns input for table: "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### history_bool_exp

Boolean expression to filter rows from the table "history". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#history_bool_exp">history_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#history_bool_exp">history_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange_comparison_exp">tstzrange_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### history_order_by

ordering options when selecting data from "history"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### jsonb_comparison_exp

expression to compare columns of type jsonb. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_contained_in</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td>

is the column contained in the given json value

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_contains</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td>

does the column contain the given json value at the top level

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the string exist as a top-level key in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_keys_all</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td>

do all of these strings exist as top-level keys in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_keys_any</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td>

do any of these strings exist as top-level keys in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#jsonb">jsonb</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#jsonb">jsonb</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### kv_store_bool_exp

Boolean expression to filter rows from the table "kv_store". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#kv_store_bool_exp">kv_store_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#kv_store_bool_exp">kv_store_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### kv_store_order_by

ordering options when selecting data from "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_order_by">developers_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### kv_store_pk_columns_input

primary key columns input for table: "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### last_utterance_bool_exp

Boolean expression to filter rows from the table "last_utterance". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#last_utterance_bool_exp">last_utterance_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#last_utterance_bool_exp">last_utterance_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### last_utterance_order_by

ordering options when selecting data from "last_utterance"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### ltree_comparison_exp

expression to compare columns of type ltree. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#ltree">ltree</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#ltree">ltree</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#ltree">ltree</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### money_comparison_exp

expression to compare columns of type money. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#money">money</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#money">money</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#money">money</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### speaker_type_enum_enum_comparison_exp

expression to compare columns of type speaker_type_enum_enum. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### timestamptz_comparison_exp

expression to compare columns of type timestamptz. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### tstzrange_comparison_exp

expression to compare columns of type tstzrange. All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#tstzrange">tstzrange</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#tstzrange">tstzrange</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_arr_rel_insert_input

input type for inserting array relation for remote table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#utterances_insert_input">utterances_insert_input</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_bool_exp

Boolean expression to filter rows from the table "utterances". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#utterances_bool_exp">utterances_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#utterances_bool_exp">utterances_bool_exp</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum_comparison_exp">speaker_type_enum_enum_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_insert_input

input type for inserting data into table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_obj_rel_insert_input">conversations_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_obj_rel_insert_input

input type for inserting object relation for remote table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#utterances_insert_input">utterances_insert_input</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_order_by

ordering options when selecting data from "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_set_input

input type for updating data in table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### Enums

#### ACEOutputType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>drs</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drshtml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drspp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drsxml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fol</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlfss</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlfsspp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlrdf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlxml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase1</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase2</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pnf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ruleml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxd</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxdpp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxpp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>tokens</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>tptp</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### AudioEncoding

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AUDIO_ENCODING_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LINEAR16</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MP3</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OGG_OPUS</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### Encoding

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AMR</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>AMR_WB</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ENCODING_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FLAC</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LINEAR16</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MP3</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MULAW</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OGG_OPUS</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SPEEX_WITH_HEADER_BYTE</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### InteractionType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>DICTATION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DISCUSSION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>INTERACTION_TYPE_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PHONE_CALL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PRESENTATION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PROFESSIONALLY_PRODUCED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>VOICEMAIL</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>VOICE_SEARCH</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### MicrophoneDistance

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>FARFIELD</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MICROPHONE_DISTANCE_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MIDFIELD</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NEARFIELD</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### OriginalMediaType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AUDIO</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ORIGINAL_MEDIA_TYPE_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>VIDEO</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### RecordingDeviceType

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>OTHER_INDOOR_DEVICE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OTHER_OUTDOOR_DEVICE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PC</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PHONE_LINE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>RECORDING_DEVICE_TYPE_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SMARTPHONE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>VEHICLE</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### app_events_select_column

select columns of table "app_events"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>app_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>data_ron</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_cost</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>window</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### apps_constraint

unique or primary key constraints on table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>apps_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>apps_slug_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

#### apps_select_column

select columns of table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>developer_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>slug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### apps_update_column

update columns of table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>slug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### conversation_events_select_column

select columns of table "conversation_events"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>data_ron</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_cost</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>window</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### conversations_constraint

unique or primary key constraints on table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>sessions_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

#### conversations_select_column

select columns of table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>app_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>destroyed_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### conversations_update_column

update columns of table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### developer_events_select_column

select columns of table "developer_events"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>data_ron</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>developer_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_cost</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>window</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### developers_constraint

unique or primary key constraints on table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>developers_api_key_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_email_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_github_handle_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_uid_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

#### developers_select_column

select columns of table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>api_key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>github_handle</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uid</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### developers_update_column

update columns of table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>github_handle</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### end_user_conversations_select_column

select columns of table "end_user_conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### history_select_column

select columns of table "history"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>interval</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterances</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>window</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### kv_store_select_column

select columns of table "kv_store"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_by</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### last_utterance_select_column

select columns of table "last_utterance"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>interval</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>speaker_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterance</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

#### order_by

column ordering options

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>asc</strong></td>
<td>

in the ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_first</strong></td>
<td>

in the ascending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_last</strong></td>
<td>

in the ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>desc</strong></td>
<td>

in the descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_first</strong></td>
<td>

in the descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_last</strong></td>
<td>

in the descending order, nulls last

</td>
</tr>
</tbody>
</table>

#### speaker_type_enum_enum

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>bot</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>user</strong></td>
<td></td>
</tr>
</tbody>
</table>

#### utterances_select_column

select columns of table "utterances"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>normalized_utterance</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>speaker_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>timestamp</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterance</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### Scalars

#### Boolean

#### Float

#### ID

#### Int

#### String

#### UUID

Leverages the internal Python implmeentation of UUID (uuid.UUID) to provide native UUID objects
in fields, resolvers and input.

#### app_status

#### jsonb

#### ltree

#### money

#### timestamptz

#### tstzrange


### Interfaces


#### Container

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentiment</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

A scalar value indicating the positivity or negativity of the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>
