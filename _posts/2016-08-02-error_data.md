## ERROR DATA
* errordata is a stack with depth errordata_stack_depth, errfinish, elog_finish and elog_dismiss would decrease this number; errfinish would be called by pg_re_throw(PG_RE_THROW), ereport, and then, if there are new coming ereports, then entries in the stack would be overriden.