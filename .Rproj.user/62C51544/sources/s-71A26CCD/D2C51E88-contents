use_typed <- function(export = TRUE) {
  usethis:::check_is_package("use_typed()")
  usethis:::check_uses_roxygen("use_typed()")
  usethis:::use_dependency("typed", "Imports")

  if(usethis:::has_package_doc()) {
    roxygen_ns_append("@importFrom typed ?") && roxygen_update()
    return(invisible(TRUE))
  }

  usethis:::ui_todo("Copy and paste this line into some roxygen header, then run \\\n    {usethis:::ui_code('devtools::document()')}:")
  usethis:::ui_code_block("#' @importFrom typed ?", copy = FALSE)
}
