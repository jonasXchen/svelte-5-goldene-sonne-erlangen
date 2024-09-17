<script>
  import {
    PUBLIC_ENTITY_CITY,
    PUBLIC_ENTITY_NAME,
    PUBLIC_ENTITY_STREET,
    PUBLIC_ENTITY_TEL,
  } from "$lib/constants";
</script>

<div class="gap-4 p-16 space-y-4 text-sm font-light text-black bg-white">
  <h1>IMPRESSUM</h1>
  <div>
    {#if PUBLIC_ENTITY_NAME}
      <p>{PUBLIC_ENTITY_NAME}</p>
    {/if}
    {#if PUBLIC_ENTITY_STREET && PUBLIC_ENTITY_CITY}
      <p>{PUBLIC_ENTITY_STREET}, {PUBLIC_ENTITY_CITY}</p>
    {/if}
    {#if PUBLIC_ENTITY_TEL}
      <p>{PUBLIC_ENTITY_TEL}</p>
    {/if}
  </div>

  <h3>Disclaimer</h3>
  <div>
    <li>Content</li>
    <p>
      The author reserves the right not to be responsible for the topicality,
      correctness, completeness or quality of the information provided.
      Liability claims regarding damage caused by the use of any information
      provided, including any kind of information which is incomplete or
      incorrect, will therefore be rejected. All offers are not-binding and
      without obligation. Parts of the pages or the complete publication
      including all offers and information might be extended, changed or partly
      or completely deleted by the author without separate announcement.
    </p>
  </div>
  <div>
    <li>Referrals and links</li>
    <p>
      The author is not responsible for any contents linked or referred to from
      his pages – unless he has full knowledge of illegal contents and would be
      able to prevent the visitors of his site from viewing those pages. If any
      damage occurs by the use of information presented there, only the author
      of the respective pages might be liable, not the one who has linked to
      these pages. Furthermore the author is not liable for any postings or
      messages published by users of discussion boards, guestbooks or mailing
      lists provided on his page.
    </p>
  </div>
  <div>
    <li>Copyright</li>
    <p>
      The author intended not to use any copyrighted material for the
      publication or, if not possible, to indicate the copyright of the
      respective object. The copyright for any material created by the author is
      reserved. Any duplication or use of objects such as diagrams, sounds or
      texts in other electronic or printed publications is not permitted without
      the author’s agreement.
    </p>
  </div>
  <div>
    <li>Privacy policy</li>
    <p>
      If the opportunity for the input of personal or business data (email
      addresses, name, addresses) is given, the input of these data takes place
      voluntarily. The use and payment of all offered services are permitted –
      if and so far technically possible and reasonable – without specification
      of any personal data or under specification of anonymized data or an
      alias. The use of published postal addresses, telephone or fax numbers and
      email addresses for marketing purposes is prohibited, offenders sending
      unwanted spam messages will be punished.
    </p>
  </div>
  <div>
    <li>Legal validity of this disclaimer</li>
    <p>
      This disclaimer is to be regarded as part of the internet publication
      which you were referred from. If sections or individual terms of this
      statement are not legal or correct, the content or validity of the other
      parts remain uninfluenced by this fact.
    </p>
  </div>
</div>
