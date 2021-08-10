
#' Regex Match Operator
#'
#' @param lhs left-hand side argument
#' @param rhs right-hand side argument
#'
#' @return Logical
#'
#' @export

`%=~%` <- function(lhs, rhs) {

  lhs <- eval(substitute(lhs))
  rhs <- eval(substitute(rhs))

  if(any(is.numeric(c(lhs, rhs)))) rlang::abort("One of the arguments is not a String nor a Regex")

  stringi::stri_detect(
    str = lhs,
    regex = rhs
    )
}


