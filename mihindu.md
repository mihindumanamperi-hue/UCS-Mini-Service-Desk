const filtered = tickets.filter((t) => {
  return (
    t.title.toLowerCase().includes(search.toLowerCase()) &&
    (statusFilter ? t.status === statusFilter : true) &&
    (priorityFilter ? t.priority === priorityFilter : true)
  );
});
