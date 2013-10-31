cmake_minimum_required(VERSION 2.8)

project(DaxReport2013 NONE)

include(UseLATEX.cmake)

set(images
  SANDimages/DOEbwlogo.pdf
  SANDimages/snllineblk.pdf
  SANDimages/SANDbackground.png
  )

set(input_docs
  )

add_latex_document(DaxReport2013.tex
  INPUTS ${input_docs}
  IMAGES ${images}
  )