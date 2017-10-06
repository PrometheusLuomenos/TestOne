# Definitions

**Feature** A feature is a unit of work which is "feature complete", meaning it contains a sufficient range of functionality so as to be deployable to production. All features should have a unique design document which should be apporved by a customer before beginning on development of the first story.

**User Story** A user story is a component of a feature which can be developed and merged with development over the course of a single sprint. User stories are estimated using points, never exceeding 20 points.
* **Task** A task is a unit of work that represents a discreet amount of work which a single person can complete in less than two days. Tasks are estimated in hours which should be updated on a daily basis while those tasks are active. Tasks are primarily managed by the "doers", so developers are responsible for creating the task, estimating effort, and burning down the tasks.
* **Bug** A bug is a unit of work similar to a task, but represents unplanned work which was identified over the course of unit testing or QA testing.

**Issue** If a defect is found after code is delivered to UAT, but before code has been promoted to Production. Because issues are necessarily defects which were missed during SVA testing, it is tracked differently. Issues live alongside Stories in work item tracking and should be ranked in priority along with stories. An issue that prevents promotion of a feature should be included as a child of that feature and marked as preventing promotion.


# Features, Stories, and Sizing
Features, Stories, and Tasks are the basic units of work. These units of work are defined both by how they fit into source control and the level of effort required to complete them. A feature work item is primarily defined as corresponding feature branch in a Git repository, whereas a story represents a unit of work which can be completed in a single sprint. But because some stories are standalone and do not fit into a larger project (e.g. Bug fixes), unparented stories will correspond to a single feature branch in code.

Stories can be independently deployed and tested and completed, however the feature is only done when the branch is merged back into the development mainline. From this point, the code will be assigned a version and become eligible for deployment to integrated testing environments. (Unparented stories are done when the corresponding feature branch is merged.)
