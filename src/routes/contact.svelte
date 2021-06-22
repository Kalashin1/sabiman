<script>
  import ContactDetails from '../components/contacts/Details.svelte'
  import Breadcrumb from '../components/about/Page-Title.svelte'
  const currentPage = 'Contact'
</script>

<Breadcrumb {currentPage} />
<ContactDetails />