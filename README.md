{
  "$id": "https://schemas.amazon.com/selling-partners/definitions/product-types/schema/v1/MANUAL_FOOD_MILL_GRINDER",
  "type": "object",
  "$defs": {
    "language_tag": {
      "type": "string",
      "anyOf": [
        {
          "type": "string"
        },
        {
          "enum": [
            "en_US"
          ],
          "type": "string",
          "enumNames": [
            "English (United States)"
          ]
        }
      ],
      "hidden": true,
      "default": "en_US",
      "editable": false,
      "examples": [
        "English (United States)"
      ]
    },
    "marketplace_id": {
      "type": "string",
      "anyOf": [
        {
          "type": "string"
        },
        {
          "enum": [
            "ATVPDKIKX0DER"
          ],
          "type": "string",
          "enumNames": [
            "Amazon.com"
          ]
        }
      ],
      "hidden": true,
      "default": "ATVPDKIKX0DER",
      "editable": false,
      "examples": [
        "Amazon.com"
      ]
    }
  },
  "allOf": [
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "merchant_suggested_asin"
                  ],
                  "properties": {
                    "merchant_suggested_asin": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "supplier_declared_has_product_identifier_exemption"
                ],
                "properties": {
                  "supplier_declared_has_product_identifier_exemption": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            false
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "merchant_suggested_asin"
                  ],
                  "properties": {
                    "merchant_suggested_asin": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "supplier_declared_has_product_identifier_exemption"
                ],
                "properties": {
                  "supplier_declared_has_product_identifier_exemption": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            false
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "merchant_suggested_asin"
                  ],
                  "properties": {
                    "merchant_suggested_asin": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "supplier_declared_has_product_identifier_exemption"
                  ],
                  "properties": {
                    "supplier_declared_has_product_identifier_exemption": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "merchant_suggested_asin"
                  ],
                  "properties": {
                    "merchant_suggested_asin": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "supplier_declared_has_product_identifier_exemption"
                  ],
                  "properties": {
                    "supplier_declared_has_product_identifier_exemption": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "externally_assigned_product_identifier"
        ]
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "externally_assigned_product_identifier"
                  ],
                  "properties": {
                    "externally_assigned_product_identifier": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "supplier_declared_has_product_identifier_exemption"
                ],
                "properties": {
                  "supplier_declared_has_product_identifier_exemption": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            false
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "externally_assigned_product_identifier"
                  ],
                  "properties": {
                    "externally_assigned_product_identifier": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "supplier_declared_has_product_identifier_exemption"
                ],
                "properties": {
                  "supplier_declared_has_product_identifier_exemption": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            false
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "externally_assigned_product_identifier"
                  ],
                  "properties": {
                    "externally_assigned_product_identifier": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "supplier_declared_has_product_identifier_exemption"
                  ],
                  "properties": {
                    "supplier_declared_has_product_identifier_exemption": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "externally_assigned_product_identifier"
                  ],
                  "properties": {
                    "externally_assigned_product_identifier": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "supplier_declared_has_product_identifier_exemption"
                  ],
                  "properties": {
                    "supplier_declared_has_product_identifier_exemption": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "merchant_suggested_asin"
        ]
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "package_level"
                ],
                "properties": {
                  "package_level": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            "case",
                            "pallet"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "package_level"
                ],
                "properties": {
                  "package_level": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            "case",
                            "pallet"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "package_contains_sku"
        ]
      }
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "model_number"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "MODEL_NUMBER/SIZE",
                            "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
                            "MODEL/SIZE_NAME",
                            "MODEL"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "model_number"
            ]
          }
        }
      ]
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "model_name"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "MODEL_NAME/TEAM_NAME",
                            "MODEL_NAME"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "model_name"
            ]
          }
        }
      ]
    },
    {
      "if": {
        "anyOf": [
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "items": {
                    "required": [
                      "value"
                    ]
                  }
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "care_instructions",
          "included_components",
          "manufacturer"
        ]
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "allOf": [
                {
                  "required": [
                    "fulfillment_channel_code"
                  ],
                  "properties": {
                    "fulfillment_channel_code": {
                      "enum": [
                        "DEFAULT"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "is_inventory_available"
                    ]
                  }
                }
              ]
            },
            "then": {
              "required": [
                "quantity"
              ]
            }
          }
        }
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "not": {
                "allOf": [
                  {
                    "required": [
                      "fulfillment_channel_code"
                    ],
                    "properties": {
                      "fulfillment_channel_code": {
                        "enum": [
                          "DEFAULT"
                        ]
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "is_inventory_available"
                      ]
                    }
                  }
                ]
              }
            },
            "then": {
              "not": {
                "required": [
                  "quantity"
                ]
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "not": {
                "required": [
                  "fulfillment_channel_code"
                ],
                "properties": {
                  "fulfillment_channel_code": {
                    "enum": [
                      "DEFAULT"
                    ]
                  }
                }
              }
            },
            "then": {
              "not": {
                "required": [
                  "lead_time_to_ship_max_days"
                ]
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "not": {
                "required": [
                  "fulfillment_channel_code"
                ],
                "properties": {
                  "fulfillment_channel_code": {
                    "enum": [
                      "DEFAULT"
                    ]
                  }
                }
              }
            },
            "then": {
              "not": {
                "required": [
                  "restock_date"
                ]
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "allOf": [
                {
                  "required": [
                    "fulfillment_channel_code"
                  ],
                  "properties": {
                    "fulfillment_channel_code": {
                      "enum": [
                        "DEFAULT"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "quantity"
                    ]
                  }
                }
              ]
            },
            "then": {
              "required": [
                "is_inventory_available"
              ]
            }
          }
        }
      }
    },
    {
      "properties": {
        "fulfillment_availability": {
          "items": {
            "if": {
              "not": {
                "allOf": [
                  {
                    "required": [
                      "fulfillment_channel_code"
                    ],
                    "properties": {
                      "fulfillment_channel_code": {
                        "enum": [
                          "DEFAULT"
                        ]
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "quantity"
                      ]
                    }
                  }
                ]
              }
            },
            "then": {
              "not": {
                "required": [
                  "is_inventory_available"
                ]
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "allOf": [
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "skip_offer"
              ],
              "properties": {
                "skip_offer": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          true
                        ]
                      }
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "fulfillment_availability"
        ]
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "map_price": {
                "properties": {
                  "schedule": {
                    "if": {
                      "required": [
                        "currency"
                      ],
                      "properties": {
                        "currency": {
                          "enum": [
                            "JPY"
                          ]
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "value_with_tax": {
                          "multipleOf": 1
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "anyOf": [
                {
                  "required": [
                    "audience"
                  ],
                  "properties": {
                    "audience": {
                      "enum": [
                        "ALL"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "audience"
                    ]
                  }
                }
              ]
            },
            "else": {
              "not": {
                "required": [
                  "map_price"
                ]
              }
            },
            "then": {
              "properties": {
                "map_price": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "our_price": {
                "properties": {
                  "schedule": {
                    "if": {
                      "required": [
                        "currency"
                      ],
                      "properties": {
                        "currency": {
                          "enum": [
                            "JPY"
                          ]
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "value_with_tax": {
                          "multipleOf": 1
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "required": [
                "discounted_price"
              ],
              "properties": {
                "discounted_price": {
                  "items": {
                    "required": [
                      "schedule"
                    ],
                    "properties": {
                      "schedule": {
                        "items": {
                          "required": [
                            "value_with_tax"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            },
            "then": {
              "required": [
                "our_price"
              ],
              "properties": {
                "our_price": {
                  "minItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "anyOf": [
                {
                  "required": [
                    "audience"
                  ],
                  "properties": {
                    "audience": {
                      "enum": [
                        "ALL"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "audience"
                    ]
                  }
                }
              ]
            },
            "else": {
              "not": {
                "required": [
                  "automated_pricing_merchandising_rule_plan"
                ]
              }
            },
            "then": {
              "properties": {
                "automated_pricing_merchandising_rule_plan": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "minimum_seller_allowed_price": {
                "properties": {
                  "schedule": {
                    "if": {
                      "required": [
                        "currency"
                      ],
                      "properties": {
                        "currency": {
                          "enum": [
                            "JPY"
                          ]
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "value_with_tax": {
                          "multipleOf": 1
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "anyOf": [
                {
                  "required": [
                    "audience"
                  ],
                  "properties": {
                    "audience": {
                      "enum": [
                        "ALL"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "audience"
                    ]
                  }
                }
              ]
            },
            "then": {
              "properties": {
                "minimum_seller_allowed_price": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "maximum_seller_allowed_price": {
                "properties": {
                  "schedule": {
                    "if": {
                      "required": [
                        "currency"
                      ],
                      "properties": {
                        "currency": {
                          "enum": [
                            "JPY"
                          ]
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "value_with_tax": {
                          "multipleOf": 1
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "anyOf": [
                {
                  "required": [
                    "audience"
                  ],
                  "properties": {
                    "audience": {
                      "enum": [
                        "ALL"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "audience"
                    ]
                  }
                }
              ]
            },
            "then": {
              "properties": {
                "maximum_seller_allowed_price": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "discounted_price": {
                "properties": {
                  "schedule": {
                    "if": {
                      "required": [
                        "currency"
                      ],
                      "properties": {
                        "currency": {
                          "enum": [
                            "JPY"
                          ]
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "value_with_tax": {
                          "multipleOf": 1
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "if": {
              "anyOf": [
                {
                  "required": [
                    "audience"
                  ],
                  "properties": {
                    "audience": {
                      "enum": [
                        "ALL"
                      ]
                    }
                  }
                },
                {
                  "not": {
                    "required": [
                      "audience"
                    ]
                  }
                }
              ]
            },
            "else": {
              "not": {
                "required": [
                  "discounted_price"
                ]
              }
            },
            "then": {
              "properties": {
                "discounted_price": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "purchasable_offer": {
          "items": {
            "properties": {
              "quantity_discount_plan": {
                "properties": {
                  "schedule": {
                    "properties": {
                      "levels": {
                        "if": {
                          "required": [
                            "currency"
                          ],
                          "properties": {
                            "currency": {
                              "enum": [
                                "JPY"
                              ]
                            }
                          }
                        },
                        "then": {
                          "properties": {
                            "value": {
                              "multipleOf": 1
                            }
                          }
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "purchasable_offer"
        ],
        "properties": {
          "purchasable_offer": {
            "contains": {
              "required": [
                "quantity_discount_plan"
              ],
              "properties": {
                "quantity_discount_plan": {
                  "contains": {
                    "required": [
                      "schedule"
                    ],
                    "properties": {
                      "schedule": {
                        "contains": {
                          "required": [
                            "discount_type"
                          ],
                          "properties": {
                            "discount_type": {
                              "enum": [
                                "percent"
                              ]
                            }
                          }
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "purchasable_offer": {
            "items": {
              "properties": {
                "quantity_discount_plan": {
                  "properties": {
                    "schedule": {
                      "properties": {
                        "levels": {
                          "properties": {
                            "value": {
                              "maximum": 99
                            }
                          }
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "skip_offer"
                  ],
                  "properties": {
                    "skip_offer": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              true
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "skip_offer"
                  ],
                  "properties": {
                    "skip_offer": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              true
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "condition_type"
        ]
      }
    },
    {
      "properties": {
        "list_price": {
          "items": {
            "if": {
              "required": [
                "currency"
              ]
            },
            "then": {
              "required": [
                "value"
              ]
            }
          }
        }
      }
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "list_price"
            ]
          }
        },
        {
          "if": {
            "anyOf": [
              {
                "allOf": [
                  {
                    "not": {
                      "required": [
                        "parentage_level"
                      ],
                      "properties": {
                        "parentage_level": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "parent"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "parentage_level"
                      ],
                      "properties": {
                        "parentage_level": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "skip_offer"
                      ],
                      "properties": {
                        "skip_offer": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  true
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  }
                ]
              },
              {
                "allOf": [
                  {
                    "not": {
                      "required": [
                        "parentage_level"
                      ],
                      "properties": {
                        "parentage_level": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "parent"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "parentage_level"
                      ],
                      "properties": {
                        "parentage_level": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "parent"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  },
                  {
                    "not": {
                      "required": [
                        "skip_offer"
                      ],
                      "properties": {
                        "skip_offer": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  true
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  }
                ]
              }
            ]
          },
          "then": {
            "required": [
              "list_price"
            ]
          }
        }
      ]
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "fulfillment_availability"
                ],
                "properties": {
                  "fulfillment_availability": {
                    "contains": {
                      "required": [
                        "fulfillment_channel_code"
                      ],
                      "properties": {
                        "fulfillment_channel_code": {
                          "enum": [
                            "DEFAULT"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "skip_offer"
                  ],
                  "properties": {
                    "skip_offer": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              true
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "fulfillment_availability"
                ],
                "properties": {
                  "fulfillment_availability": {
                    "contains": {
                      "required": [
                        "fulfillment_channel_code"
                      ],
                      "properties": {
                        "fulfillment_channel_code": {
                          "enum": [
                            "DEFAULT"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "skip_offer"
                  ],
                  "properties": {
                    "skip_offer": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              true
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "merchant_shipping_group"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
                        "STYLE_NAME/COLOR_NAME",
                        "COLOR_NAME/SIZE_NAME/STYLE_NAME",
                        "STYLE_NAME",
                        "STYLE_NAME/COLOR_NAME/SIZE_NAME",
                        "STYLE_NAME/SIZE_NAME",
                        "STYLE_NAME/PATTERN_NAME",
                        "ITEM_PACKAGE_QUANTITY/STYLE_NAME",
                        "COLOR_NAME/STYLE_NAME",
                        "SIZE_NAME/STYLE_NAME"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "style"
        ]
      }
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "material"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "COLOR/MATERIAL",
                            "MATERIAL/COLOR",
                            "MATERIAL/SIZE",
                            "SIZE/MATERIAL",
                            "MATERIAL_TYPE",
                            "COLOR_NAME/MATERIAL_TYPE",
                            "MATERIAL_TYPE/SIZE_NAME",
                            "MATERIAL_TYPE/COLOR_NAME",
                            "MATERIAL_TYPE/ITEM_DISPLAY_WEIGHT",
                            "SIZE_NAME/MATERIAL_TYPE",
                            "ITEM_DISPLAY_WEIGHT/MATERIAL_TYPE"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "material"
            ]
          }
        }
      ]
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "number_of_items"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "SIZE/COLOR/NUMBER_OF_ITEMS",
                            "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
                            "COLOR_NAME/NUMBER_OF_ITEMS",
                            "NUMBER_OF_ITEMS",
                            "SIZE/NUMBER_OF_ITEMS",
                            "COLOR/NUMBER_OF_ITEMS",
                            "SIZE_NAME/NUMBER_OF_ITEMS",
                            "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "number_of_items"
            ]
          }
        }
      ]
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "ITEM_PACKAGE_QUANTITY",
                        "ITEM_PACKAGE_QUANTITY/STYLE_NAME",
                        "ITEM_PACKAGE_QUANTITY/COLOR_NAME",
                        "ITEM_PACKAGE_QUANTITY/SIZE_NAME"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "item_package_quantity"
        ]
      }
    },
    {
      "properties": {
        "color": {
          "items": {
            "if": {
              "not": {
                "required": [
                  "value"
                ]
              }
            },
            "then": {
              "required": [
                "standardized_values"
              ],
              "properties": {
                "standardized_values": {
                  "minItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "color"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "COLOR/MATERIAL",
                            "MATERIAL/COLOR",
                            "SIZE/COLOR/NUMBER_OF_ITEMS",
                            "COLOR_NAME/MATERIAL_TYPE",
                            "COLOR_NAME/SIZE_NAME",
                            "STYLE_NAME/COLOR_NAME",
                            "COLOR/SIZE",
                            "COLOR_NAME/SIZE_NAME/STYLE_NAME",
                            "MATERIAL_TYPE/COLOR_NAME",
                            "COLOR_NAME/NUMBER_OF_ITEMS",
                            "COLOR_NAME",
                            "COLOR",
                            "COLOR_NAME/WATTAGE",
                            "STYLE_NAME/COLOR_NAME/SIZE_NAME",
                            "COLOR_NAME/ITEM_DISPLAY_WEIGHT",
                            "SIZE/COLOR",
                            "COLOR/NUMBER_OF_ITEMS",
                            "ITEM_PACKAGE_QUANTITY/COLOR_NAME",
                            "ITEM_DISPLAY_WEIGHT/COLOR_NAME",
                            "COLOR_NAME/STYLE_NAME",
                            "SIZE_NAME/COLOR_NAME",
                            "COLOR/WATTAGE",
                            "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "color"
            ]
          }
        }
      ]
    },
    {
      "allOf": [
        {
          "if": {
            "anyOf": [
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "size"
            ]
          }
        },
        {
          "if": {
            "allOf": [
              {
                "required": [
                  "child_parent_sku_relationship"
                ],
                "properties": {
                  "child_parent_sku_relationship": {
                    "items": {
                      "required": [
                        "parent_sku"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "required": [
                  "variation_theme"
                ],
                "properties": {
                  "variation_theme": {
                    "contains": {
                      "required": [
                        "name"
                      ],
                      "properties": {
                        "name": {
                          "enum": [
                            "MATERIAL/SIZE",
                            "MODEL_NUMBER/SIZE",
                            "SIZE/COLOR/NUMBER_OF_ITEMS",
                            "SIZE/MATERIAL",
                            "TEAM_NAME/SIZE_NAME",
                            "ITEM_DISPLAY_WEIGHT/SIZE_NAME",
                            "COLOR_NAME/SIZE_NAME",
                            "COLOR/SIZE",
                            "COLOR_NAME/SIZE_NAME/STYLE_NAME",
                            "MATERIAL_TYPE/SIZE_NAME",
                            "SIZE_NAME",
                            "STYLE_NAME/COLOR_NAME/SIZE_NAME",
                            "SIZE/UNIT_COUNT",
                            "MODEL/SIZE_NAME",
                            "SIZE_NAME/ITEM_DISPLAY_WEIGHT",
                            "SIZE/NUMBER_OF_ITEMS",
                            "SIZE/COLOR",
                            "PATTERN_NAME/SIZE_NAME",
                            "STYLE_NAME/SIZE_NAME",
                            "SIZE",
                            "SIZE_NAME/PART_NUMBER",
                            "ITEM_PACKAGE_QUANTITY/SIZE_NAME",
                            "SIZE_NAME/COLOR_NAME",
                            "SIZE_NAME/NUMBER_OF_ITEMS",
                            "SIZE_NAME/UNIT_COUNT",
                            "SIZE_NAME/MATERIAL_TYPE",
                            "SIZE_NAME/STYLE_NAME",
                            "FLAVOR/SIZE",
                            "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS",
                            "SIZE_NAME/PATTERN_NAME"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          "then": {
            "required": [
              "size"
            ]
          }
        }
      ]
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
                        "SIZE_NAME/PART_NUMBER"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "part_number"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "FLAVOR_NAME",
                        "FLAVOR/SIZE"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "flavor"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "COLOR_NAME/WATTAGE",
                        "WATTAGE",
                        "COLOR/WATTAGE"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "wattage"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "VOLTAGE"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "voltage"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "CUSTOMER_PACKAGE_TYPE"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "customer_package_type"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "PATTERN_NAME/SIZE_NAME",
                        "STYLE_NAME/PATTERN_NAME",
                        "PATTERN_NAME",
                        "PATTERN",
                        "SIZE_NAME/PATTERN_NAME"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "pattern"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "SIZE/UNIT_COUNT",
                        "SIZE_NAME/UNIT_COUNT"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "unit_count"
        ]
      }
    },
    {
      "if": {
        "required": [
          "league_name"
        ],
        "properties": {
          "league_name": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "NASCAR",
                    "nascar",
                    "ناسكار"
                  ]
                }
              }
            }
          }
        }
      },
      "else": {
        "if": {
          "required": [
            "league_name"
          ],
          "properties": {
            "league_name": {
              "contains": {
                "required": [
                  "value"
                ],
                "properties": {
                  "value": {
                    "enum": [
                      "eスポーツ",
                      "E-Sports (sport elettronici)",
                      "E-sport",
                      "E-Sports",
                      "ألعاب إلكترونية",
                      "E-Sport",
                      "e_sports",
                      "Deportes electrónicos"
                    ]
                  }
                }
              }
            }
          }
        },
        "else": {
          "if": {
            "required": [
              "league_name"
            ],
            "properties": {
              "league_name": {
                "contains": {
                  "required": [
                    "value"
                  ],
                  "properties": {
                    "value": {
                      "enum": [
                        "Pro Wrestling League",
                        "Liga de lucha libre profesional",
                        "インド/プロレスリーグ",
                        "Liga Profissional de Luta Livre",
                        "pro_wrestling_league",
                        "Pro Wrestling Ligan",
                        "دوري المصارعة للمحترفين"
                      ]
                    }
                  }
                }
              }
            }
          },
          "else": {
            "if": {
              "required": [
                "league_name"
              ],
              "properties": {
                "league_name": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "Formel 1",
                          "Formuła 1",
                          "formula_1",
                          "Fórmula 1",
                          "Formula 1",
                          "فورمولا 1",
                          "Formule 1",
                          "フォーミュラ1"
                        ]
                      }
                    }
                  }
                }
              }
            },
            "else": {
              "if": {
                "required": [
                  "league_name"
                ],
                "properties": {
                  "league_name": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            "I-ligan",
                            "I-League",
                            "インド/Iリーグ",
                            "Liga I",
                            "i_league",
                            "الدوري الهندي للمحترفين"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              "else": {
                "if": {
                  "required": [
                    "league_name"
                  ],
                  "properties": {
                    "league_name": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "Japanischer Baseball",
                              "Campionato di baseball giapponese",
                              "Baseball japonais",
                              "Béisbol japonés",
                              "日本/セ・パリーグ・高校野球",
                              "Japanese Baseball",
                              "Japans honkbal",
                              "japanese_baseball",
                              "Japansk baseboll",
                              "البيسبول الياباني",
                              "Japoński baseball",
                              "Beisebol japonês"
                            ]
                          }
                        }
                      }
                    }
                  }
                },
                "else": {
                  "if": {
                    "required": [
                      "league_name"
                    ],
                    "properties": {
                      "league_name": {
                        "contains": {
                          "required": [
                            "value"
                          ],
                          "properties": {
                            "value": {
                              "enum": [
                                "イギリス/サッカー",
                                "English Football",
                                "Engels voetbal",
                                "Football britannique",
                                "كرة القدم الإنجليزية",
                                "Angielska piłka nożna",
                                "english_football",
                                "English Soccer",
                                "British Football",
                                "Calcio inglese",
                                "Futebol inglês",
                                "Engelsk fotboll",
                                "Englischer Fußball",
                                "Fútbol inglés"
                              ]
                            }
                          }
                        }
                      }
                    }
                  },
                  "else": {
                    "if": {
                      "required": [
                        "league_name"
                      ],
                      "properties": {
                        "league_name": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "الاتحاد الدولي للمصارعة",
                                  "WUSA",
                                  "wusa"
                                ]
                              }
                            }
                          }
                        }
                      }
                    },
                    "else": {
                      "if": {
                        "required": [
                          "league_name"
                        ],
                        "properties": {
                          "league_name": {
                            "contains": {
                              "required": [
                                "value"
                              ],
                              "properties": {
                                "value": {
                                  "enum": [
                                    "Première Ligue canadienne",
                                    "Kanadensisk premiärliga",
                                    "Canadian Premier League",
                                    "Liga Premier Canadense",
                                    "canadian_premier_league",
                                    "Premiere League canadiense",
                                    "Liga Premier canadiense",
                                    "Premier League Kanada",
                                    "Canadian Premiere League",
                                    "الدوري الكندي الممتاز",
                                    "カナダ/プレミアリーグ",
                                    "Kanadyjska Premiere League"
                                  ]
                                }
                              }
                            }
                          }
                        }
                      },
                      "else": {
                        "if": {
                          "required": [
                            "league_name"
                          ],
                          "properties": {
                            "league_name": {
                              "contains": {
                                "required": [
                                  "value"
                                ],
                                "properties": {
                                  "value": {
                                    "enum": [
                                      "Fútbol español",
                                      "Spanish Football",
                                      "كرة القدم الاسبانية",
                                      "Calcio spagnolo",
                                      "Futebol espanhol",
                                      "Football espagnol",
                                      "spanish_football",
                                      "Hiszpańska piłka nożna",
                                      "Spanish Soccer",
                                      "Spanischer Fußball",
                                      "Spaans voetbal",
                                      "Spansk fotboll",
                                      "スペイン/サッカー"
                                    ]
                                  }
                                }
                              }
                            }
                          }
                        },
                        "else": {
                          "if": {
                            "required": [
                              "league_name"
                            ],
                            "properties": {
                              "league_name": {
                                "contains": {
                                  "required": [
                                    "value"
                                  ],
                                  "properties": {
                                    "value": {
                                      "enum": [
                                        "Canadian Football League",
                                        "Liga Canadense de Futebol",
                                        "Kanadyjska Liga Piłkarska",
                                        "canadian_football_league",
                                        "Ligue canadienne de football",
                                        "Kanadensisk fotbollsliga",
                                        "الدوري الكندي لكرة القدم",
                                        "Kanadische Fußballliga",
                                        "カナディアン・フットボール・リーグ",
                                        "Liga de fútbol canadiense"
                                      ]
                                    }
                                  }
                                }
                              }
                            }
                          },
                          "else": {
                            "if": {
                              "required": [
                                "league_name"
                              ],
                              "properties": {
                                "league_name": {
                                  "contains": {
                                    "required": [
                                      "value"
                                    ],
                                    "properties": {
                                      "value": {
                                        "enum": [
                                          "دوري كرة السلة الأميركي للمحترفين",
                                          "nba",
                                          "NBA"
                                        ]
                                      }
                                    }
                                  }
                                }
                              }
                            },
                            "else": {
                              "if": {
                                "required": [
                                  "league_name"
                                ],
                                "properties": {
                                  "league_name": {
                                    "contains": {
                                      "required": [
                                        "value"
                                      ],
                                      "properties": {
                                        "value": {
                                          "enum": [
                                            "Minor League Honkbal",
                                            "minor_league_baseball",
                                            "Béisbol de ligas menores",
                                            "Minor League Baseball",
                                            "Liga Menor de Beisebol",
                                            "Ligue mineure de baseball",
                                            "アメリカ/マイナーリーグ",
                                            "دوري البيسبول المصغر"
                                          ]
                                        }
                                      }
                                    }
                                  }
                                }
                              },
                              "else": {
                                "if": {
                                  "required": [
                                    "league_name"
                                  ],
                                  "properties": {
                                    "league_name": {
                                      "contains": {
                                        "required": [
                                          "value"
                                        ],
                                        "properties": {
                                          "value": {
                                            "enum": [
                                              "دوري الهوكي الوطني",
                                              "nhl",
                                              "NHL",
                                              "Ligue nationale de hockey"
                                            ]
                                          }
                                        }
                                      }
                                    }
                                  }
                                },
                                "else": {
                                  "if": {
                                    "required": [
                                      "league_name"
                                    ],
                                    "properties": {
                                      "league_name": {
                                        "contains": {
                                          "required": [
                                            "value"
                                          ],
                                          "properties": {
                                            "value": {
                                              "enum": [
                                                "European Basketball",
                                                "Europees basketbal",
                                                "كرة السلة الأوروبية",
                                                "european_basketball",
                                                "Baloncesto europeo",
                                                "Europeisk basket",
                                                "Lega europea di pallacanestro",
                                                "バスケットボール ユーロリーグ",
                                                "Basquete europeu",
                                                "Europejska koszykówka",
                                                "Basketball européen",
                                                "Europäischer Basketball"
                                              ]
                                            }
                                          }
                                        }
                                      }
                                    }
                                  },
                                  "else": {
                                    "if": {
                                      "required": [
                                        "league_name"
                                      ],
                                      "properties": {
                                        "league_name": {
                                          "contains": {
                                            "required": [
                                              "value"
                                            ],
                                            "properties": {
                                              "value": {
                                                "enum": [
                                                  "Liga Premier de Badminton",
                                                  "インド/バドミントンリーグ",
                                                  "Premier Badminton League",
                                                  "premier_badminton_league",
                                                  "Liga Premier de Bádminton",
                                                  "Premier Badminton Ligan",
                                                  "الدوري الممتاز لكرة الريشة"
                                                ]
                                              }
                                            }
                                          }
                                        }
                                      }
                                    },
                                    "else": {
                                      "if": {
                                        "required": [
                                          "league_name"
                                        ],
                                        "properties": {
                                          "league_name": {
                                            "contains": {
                                              "required": [
                                                "value"
                                              ],
                                              "properties": {
                                                "value": {
                                                  "enum": [
                                                    "Otros equipos de fútbol",
                                                    "Other Soccer Leagues",
                                                    "other_football_leagues",
                                                    "サッカーリーグ/その他",
                                                    "Otras ligas de fútbol",
                                                    "Inne ligi piłkarskie",
                                                    "Andere voetbalcompetities",
                                                    "Autres équipes de football",
                                                    "Mehr Fußballmannschaften",
                                                    "More Football Leagues",
                                                    "Outras ligas de futebol",
                                                    "بطولات كرة القدم الأخرى",
                                                    "Altre squadre di calcio",
                                                    "Andra fotbollsligor"
                                                  ]
                                                }
                                              }
                                            }
                                          }
                                        }
                                      },
                                      "else": {
                                        "if": {
                                          "required": [
                                            "league_name"
                                          ],
                                          "properties": {
                                            "league_name": {
                                              "contains": {
                                                "required": [
                                                  "value"
                                                ],
                                                "properties": {
                                                  "value": {
                                                    "enum": [
                                                      "ポルトガル/サッカー",
                                                      "Portuguese Football",
                                                      "Futebol português",
                                                      "Fútbol portugués",
                                                      "Football portugais",
                                                      "Portugees voetbal",
                                                      "Portugiesischer Fußball",
                                                      "portuguese_football",
                                                      "Portugisisk fotboll",
                                                      "Portuguese Soccer",
                                                      "Portugalska piłka nożna",
                                                      "كرة القدم البرتغالية",
                                                      "Campionato di calcio portoghese"
                                                    ]
                                                  }
                                                }
                                              }
                                            }
                                          }
                                        },
                                        "else": {
                                          "if": {
                                            "required": [
                                              "league_name"
                                            ],
                                            "properties": {
                                              "league_name": {
                                                "contains": {
                                                  "required": [
                                                    "value"
                                                  ],
                                                  "properties": {
                                                    "value": {
                                                      "enum": [
                                                        "الدوري الأمريكي لكرة القدم",
                                                        "mls",
                                                        "MLS"
                                                      ]
                                                    }
                                                  }
                                                }
                                              }
                                            }
                                          },
                                          "else": {
                                            "if": {
                                              "required": [
                                                "league_name"
                                              ],
                                              "properties": {
                                                "league_name": {
                                                  "contains": {
                                                    "required": [
                                                      "value"
                                                    ],
                                                    "properties": {
                                                      "value": {
                                                        "enum": [
                                                          "ncaa",
                                                          "دوري الجامعات الأمريكية لكرة السلة",
                                                          "NCAA"
                                                        ]
                                                      }
                                                    }
                                                  }
                                                }
                                              }
                                            },
                                            "else": {
                                              "if": {
                                                "required": [
                                                  "league_name"
                                                ],
                                                "properties": {
                                                  "league_name": {
                                                    "contains": {
                                                      "required": [
                                                        "value"
                                                      ],
                                                      "properties": {
                                                        "value": {
                                                          "enum": [
                                                            "Campionato mondiale di calcio",
                                                            "World Cup Football",
                                                            "Wereldkampioenschap voetbal",
                                                            "Copa do Mundo de Futebol",
                                                            "World Cup Soccer",
                                                            "Mistrzostwa Świata w Piłce Nożnej",
                                                            "VM-fotboll",
                                                            "Fútbol Copa del Mundo",
                                                            "Fußballweltmeisterschaft",
                                                            "كأس العالم لكرة القدم",
                                                            "FIFAワールドカップ",
                                                            "Coupe du monde de football",
                                                            "Copa mundial de fútbol",
                                                            "world_cup_football"
                                                          ]
                                                        }
                                                      }
                                                    }
                                                  }
                                                }
                                              },
                                              "else": {
                                                "if": {
                                                  "required": [
                                                    "league_name"
                                                  ],
                                                  "properties": {
                                                    "league_name": {
                                                      "contains": {
                                                        "required": [
                                                          "value"
                                                        ],
                                                        "properties": {
                                                          "value": {
                                                            "enum": [
                                                              "Indiska Soccer-ligan",
                                                              "Indian Soccer League",
                                                              "Indian Super League",
                                                              "Indyjska Soccer League",
                                                              "Indische Fußballliga",
                                                              "インド/サッカーリーグ",
                                                              "Liga de fútbol de la India",
                                                              "Liga de fútbol india",
                                                              "indian_soccer_league",
                                                              "دوري كرة القدم الهندي",
                                                              "Liga Indiana de Futebol",
                                                              "Ligue indienne de football"
                                                            ]
                                                          }
                                                        }
                                                      }
                                                    }
                                                  }
                                                },
                                                "else": {
                                                  "if": {
                                                    "required": [
                                                      "league_name"
                                                    ],
                                                    "properties": {
                                                      "league_name": {
                                                        "contains": {
                                                          "required": [
                                                            "value"
                                                          ],
                                                          "properties": {
                                                            "value": {
                                                              "enum": [
                                                                "Equipes nationales de football",
                                                                "代表チーム",
                                                                "National Teams",
                                                                "Selecciones nacionales",
                                                                "Landslag",
                                                                "Nationale teams",
                                                                "Squadre Nazionali",
                                                                "national_teams",
                                                                "Nationale Fußballmannschaften",
                                                                "Selecciones de fútbol",
                                                                "Seleções Nacionais",
                                                                "Drużyny narodowe",
                                                                "المنتخبات الوطنية"
                                                              ]
                                                            }
                                                          }
                                                        }
                                                      }
                                                    }
                                                  },
                                                  "else": {
                                                    "if": {
                                                      "required": [
                                                        "league_name"
                                                      ],
                                                      "properties": {
                                                        "league_name": {
                                                          "contains": {
                                                            "required": [
                                                              "value"
                                                            ],
                                                            "properties": {
                                                              "value": {
                                                                "enum": [
                                                                  "メキシコ/サッカー連盟",
                                                                  "Mexican Football Federation",
                                                                  "Federação Mexicana de Futebol",
                                                                  "Mexicaanse Vereniging Van De Voetbalbond",
                                                                  "Federazione calcistica del Messico",
                                                                  "Federación Mexicana De Fútbol Asociación",
                                                                  "Federación Mexicana de Fútbol Asociación",
                                                                  "اتحاد كرة القدم المكسيكي",
                                                                  "Fédération du Mexique de football",
                                                                  "federacion_mexicana_de_futbol_ascn"
                                                                ]
                                                              }
                                                            }
                                                          }
                                                        }
                                                      }
                                                    },
                                                    "else": {
                                                      "if": {
                                                        "required": [
                                                          "league_name"
                                                        ],
                                                        "properties": {
                                                          "league_name": {
                                                            "contains": {
                                                              "required": [
                                                                "value"
                                                              ],
                                                              "properties": {
                                                                "value": {
                                                                  "enum": [
                                                                    "Football néerlandais",
                                                                    "Dutch Soccer",
                                                                    "Holenderska piłka nożna",
                                                                    "كرة القدم الهولندية",
                                                                    "Futebol holandês",
                                                                    "Fútbol holandés",
                                                                    "dutch_football",
                                                                    "Nederlands voetbal",
                                                                    "オランダ/サッカー",
                                                                    "Dutch Football",
                                                                    "Holländsk fotboll",
                                                                    "Niederländischer Fußball",
                                                                    "Campionato di calcio olandese"
                                                                  ]
                                                                }
                                                              }
                                                            }
                                                          }
                                                        }
                                                      },
                                                      "else": {
                                                        "if": {
                                                          "required": [
                                                            "league_name"
                                                          ],
                                                          "properties": {
                                                            "league_name": {
                                                              "contains": {
                                                                "required": [
                                                                  "value"
                                                                ],
                                                                "properties": {
                                                                  "value": {
                                                                    "enum": [
                                                                      "X-spel",
                                                                      "العاب اكس",
                                                                      "X-Games",
                                                                      "X Games",
                                                                      "Xゲーム",
                                                                      "x_games"
                                                                    ]
                                                                  }
                                                                }
                                                              }
                                                            }
                                                          }
                                                        },
                                                        "else": {
                                                          "if": {
                                                            "required": [
                                                              "league_name"
                                                            ],
                                                            "properties": {
                                                              "league_name": {
                                                                "contains": {
                                                                  "required": [
                                                                    "value"
                                                                  ],
                                                                  "properties": {
                                                                    "value": {
                                                                      "enum": [
                                                                        "german_football",
                                                                        "كرة القدم الألمانية",
                                                                        "Tysk fotboll",
                                                                        "Deutscher Fußball",
                                                                        "Fútbol alemán",
                                                                        "Niemiecka piłka nożna",
                                                                        "Calcio tedesco",
                                                                        "German Soccer",
                                                                        "Football allemand",
                                                                        "Futebol alemão",
                                                                        "Duits voetbal",
                                                                        "German Football",
                                                                        "ドイツ/サッカー"
                                                                      ]
                                                                    }
                                                                  }
                                                                }
                                                              }
                                                            }
                                                          },
                                                          "else": {
                                                            "if": {
                                                              "required": [
                                                                "league_name"
                                                              ],
                                                              "properties": {
                                                                "league_name": {
                                                                  "contains": {
                                                                    "required": [
                                                                      "value"
                                                                    ],
                                                                    "properties": {
                                                                      "value": {
                                                                        "enum": [
                                                                          "الدوري الوطني لكرة القدم للسيدات",
                                                                          "NWSL",
                                                                          "nwsl"
                                                                        ]
                                                                      }
                                                                    }
                                                                  }
                                                                }
                                                              }
                                                            },
                                                            "else": {
                                                              "if": {
                                                                "required": [
                                                                  "league_name"
                                                                ],
                                                                "properties": {
                                                                  "league_name": {
                                                                    "contains": {
                                                                      "required": [
                                                                        "value"
                                                                      ],
                                                                      "properties": {
                                                                        "value": {
                                                                          "enum": [
                                                                            "Pro Kabaddi League",
                                                                            "pro_kabaddi_league",
                                                                            "Pro Kabaddi Ligan",
                                                                            "دوري كبادي للمحترفين",
                                                                            "Liga Pro Kabaddi",
                                                                            "インド/プロカバディリーグ"
                                                                          ]
                                                                        }
                                                                      }
                                                                    }
                                                                  }
                                                                }
                                                              },
                                                              "else": {
                                                                "if": {
                                                                  "required": [
                                                                    "league_name"
                                                                  ],
                                                                  "properties": {
                                                                    "league_name": {
                                                                      "contains": {
                                                                        "required": [
                                                                          "value"
                                                                        ],
                                                                        "properties": {
                                                                          "value": {
                                                                            "enum": [
                                                                              "رابطة لاعبي الغولف المحترفين",
                                                                              "pga",
                                                                              "PGA",
                                                                              "PGAツアー"
                                                                            ]
                                                                          }
                                                                        }
                                                                      }
                                                                    }
                                                                  }
                                                                },
                                                                "else": {
                                                                  "if": {
                                                                    "required": [
                                                                      "league_name"
                                                                    ],
                                                                    "properties": {
                                                                      "league_name": {
                                                                        "contains": {
                                                                          "required": [
                                                                            "value"
                                                                          ],
                                                                          "properties": {
                                                                            "value": {
                                                                              "enum": [
                                                                                "Schottischer Fußball",
                                                                                "كرة القدم الاسكتلندية",
                                                                                "Skotsk fotboll",
                                                                                "Futebol escocês",
                                                                                "Football écossais",
                                                                                "Fútbol escocés",
                                                                                "Scottish Soccer",
                                                                                "Scottish Football",
                                                                                "Schots voetbal",
                                                                                "スコットランド/サッカー",
                                                                                "Szkocka piłka nożna",
                                                                                "scottish_football",
                                                                                "Campionato di calcio scozzese"
                                                                              ]
                                                                            }
                                                                          }
                                                                        }
                                                                      }
                                                                    }
                                                                  },
                                                                  "else": {
                                                                    "if": {
                                                                      "required": [
                                                                        "league_name"
                                                                      ],
                                                                      "properties": {
                                                                        "league_name": {
                                                                          "contains": {
                                                                            "required": [
                                                                              "value"
                                                                            ],
                                                                            "properties": {
                                                                              "value": {
                                                                                "enum": [
                                                                                  "Französischer Fußball",
                                                                                  "Frans voetbal",
                                                                                  "French Football",
                                                                                  "Fransk fotboll",
                                                                                  "French Soccer",
                                                                                  "Francuska piłka nożna",
                                                                                  "Calcio francese",
                                                                                  "Futebol francês",
                                                                                  "french_football",
                                                                                  "كرة القدم الفرنسية",
                                                                                  "Fútbol francés",
                                                                                  "フランス/サッカー",
                                                                                  "Football français"
                                                                                ]
                                                                              }
                                                                            }
                                                                          }
                                                                        }
                                                                      }
                                                                    },
                                                                    "else": {
                                                                      "if": {
                                                                        "required": [
                                                                          "league_name"
                                                                        ],
                                                                        "properties": {
                                                                          "league_name": {
                                                                            "contains": {
                                                                              "required": [
                                                                                "value"
                                                                              ],
                                                                              "properties": {
                                                                                "value": {
                                                                                  "enum": [
                                                                                    "LPGAツアー",
                                                                                    "lpga",
                                                                                    "رابطة لاعبات الغولف المحترفات",
                                                                                    "LPGA"
                                                                                  ]
                                                                                }
                                                                              }
                                                                            }
                                                                          }
                                                                        }
                                                                      },
                                                                      "else": {
                                                                        "if": {
                                                                          "required": [
                                                                            "league_name"
                                                                          ],
                                                                          "properties": {
                                                                            "league_name": {
                                                                              "contains": {
                                                                                "required": [
                                                                                  "value"
                                                                                ],
                                                                                "properties": {
                                                                                  "value": {
                                                                                    "enum": [
                                                                                      "لعبة الكريكيت الدولية",
                                                                                      "Międzynarodowy krykiet",
                                                                                      "Internationales Cricket",
                                                                                      "クリケット代表チーム",
                                                                                      "international_cricket",
                                                                                      "Campionato internazionale di cricket",
                                                                                      "Internationell Cricket",
                                                                                      "Cricket international",
                                                                                      "Cricket internacional",
                                                                                      "Críquete Internacional",
                                                                                      "International Cricket"
                                                                                    ]
                                                                                  }
                                                                                }
                                                                              }
                                                                            }
                                                                          }
                                                                        },
                                                                        "else": {
                                                                          "if": {
                                                                            "required": [
                                                                              "league_name"
                                                                            ],
                                                                            "properties": {
                                                                              "league_name": {
                                                                                "contains": {
                                                                                  "required": [
                                                                                    "value"
                                                                                  ],
                                                                                  "properties": {
                                                                                    "value": {
                                                                                      "enum": [
                                                                                        "Nationella Lacrosse-ligan",
                                                                                        "دوري لاكروس الوطني",
                                                                                        "ナショナル・ラクロス・リーグ",
                                                                                        "National Lacrosse League",
                                                                                        "Liga Nacional de Lacrosse",
                                                                                        "Liga nacional de lacrosse",
                                                                                        "national_lacrosse_league",
                                                                                        "Narodowa Liga Lacrosse"
                                                                                      ]
                                                                                    }
                                                                                  }
                                                                                }
                                                                              }
                                                                            }
                                                                          },
                                                                          "else": {
                                                                            "if": {
                                                                              "required": [
                                                                                "league_name"
                                                                              ],
                                                                              "properties": {
                                                                                "league_name": {
                                                                                  "contains": {
                                                                                    "required": [
                                                                                      "value"
                                                                                    ],
                                                                                    "properties": {
                                                                                      "value": {
                                                                                        "enum": [
                                                                                          "hockey_india_league",
                                                                                          "Liga De Hóquei Indiano",
                                                                                          "Hockey India League",
                                                                                          "Hokejowa liga indyjska",
                                                                                          "Liga India de Hockey",
                                                                                          "ホッケーインドリーグ",
                                                                                          "Liga india de hockey",
                                                                                          "Indiens hockeyliga",
                                                                                          "دوري الهوكي الهندي",
                                                                                          "Campionato di hockey indiano"
                                                                                        ]
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                }
                                                                              }
                                                                            },
                                                                            "else": {
                                                                              "if": {
                                                                                "required": [
                                                                                  "league_name"
                                                                                ],
                                                                                "properties": {
                                                                                  "league_name": {
                                                                                    "contains": {
                                                                                      "required": [
                                                                                        "value"
                                                                                      ],
                                                                                      "properties": {
                                                                                        "value": {
                                                                                          "enum": [
                                                                                            "كرة القدم الايطالية",
                                                                                            "italian_football",
                                                                                            "Italienischer Fußball",
                                                                                            "Italian Soccer",
                                                                                            "Włoska piłka nożna",
                                                                                            "Italiensk fotboll",
                                                                                            "Football italien",
                                                                                            "Calcio italiano",
                                                                                            "Italiaans voetbal",
                                                                                            "Fútbol italiano",
                                                                                            "Futebol italiano",
                                                                                            "Italian Football",
                                                                                            "イタリア/サッカー"
                                                                                          ]
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                }
                                                                              },
                                                                              "else": {
                                                                                "if": {
                                                                                  "required": [
                                                                                    "league_name"
                                                                                  ],
                                                                                  "properties": {
                                                                                    "league_name": {
                                                                                      "contains": {
                                                                                        "required": [
                                                                                          "value"
                                                                                        ],
                                                                                        "properties": {
                                                                                          "value": {
                                                                                            "enum": [
                                                                                              "Campionato di pallavolo professionale",
                                                                                              "دوري المحترفين للكرة الطائرة",
                                                                                              "インド/バレーボールリーグ",
                                                                                              "Pro Volleyball Ligan",
                                                                                              "Pro Volleyball League",
                                                                                              "pro_volleyball_league",
                                                                                              "Liga Profissional de Vôlei",
                                                                                              "Liga de voleibol profesional"
                                                                                            ]
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                },
                                                                                "else": {
                                                                                  "if": {
                                                                                    "required": [
                                                                                      "league_name"
                                                                                    ],
                                                                                    "properties": {
                                                                                      "league_name": {
                                                                                        "contains": {
                                                                                          "required": [
                                                                                            "value"
                                                                                          ],
                                                                                          "properties": {
                                                                                            "value": {
                                                                                              "enum": [
                                                                                                "Japońska piłka nożna",
                                                                                                "Campionato di calcio giapponese",
                                                                                                "Japansk fotboll",
                                                                                                "Japanese Soccer",
                                                                                                "Japanischer Fußball",
                                                                                                "Japans voetbal",
                                                                                                "Japanese Football",
                                                                                                "Futebol japonês",
                                                                                                "كرة القدم اليابانية",
                                                                                                "日本/Jリーグ",
                                                                                                "Fútbol japonés",
                                                                                                "japanese_football",
                                                                                                "Football japonais"
                                                                                              ]
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  },
                                                                                  "else": {
                                                                                    "if": {
                                                                                      "required": [
                                                                                        "league_name"
                                                                                      ],
                                                                                      "properties": {
                                                                                        "league_name": {
                                                                                          "contains": {
                                                                                            "required": [
                                                                                              "value"
                                                                                            ],
                                                                                            "properties": {
                                                                                              "value": {
                                                                                                "enum": [
                                                                                                  "البيسبول الكلاسيكية العالمية",
                                                                                                  "world_baseball_classic",
                                                                                                  "Clásico mundial de béisbol",
                                                                                                  "Classique mondiale de baseball",
                                                                                                  "Wereld Honkbal Klassieker",
                                                                                                  "World Baseball Classic",
                                                                                                  "Clássico Mundial de Beisebol",
                                                                                                  "ワールドベースボールクラシック"
                                                                                                ]
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    },
                                                                                    "else": {
                                                                                      "if": {
                                                                                        "required": [
                                                                                          "league_name"
                                                                                        ],
                                                                                        "properties": {
                                                                                          "league_name": {
                                                                                            "contains": {
                                                                                              "required": [
                                                                                                "value"
                                                                                              ],
                                                                                              "properties": {
                                                                                                "value": {
                                                                                                  "enum": [
                                                                                                    "Indiska Premier-ligan",
                                                                                                    "Szkocka Premier League",
                                                                                                    "Liga Premier de la India",
                                                                                                    "Indian Premier League",
                                                                                                    "インディアン・プレミアリーグ",
                                                                                                    "الدوري الهندي الممتاز",
                                                                                                    "Liga Premier Indiana",
                                                                                                    "indian_premier_league",
                                                                                                    "Premier League india"
                                                                                                  ]
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      },
                                                                                      "else": {
                                                                                        "if": {
                                                                                          "required": [
                                                                                            "league_name"
                                                                                          ],
                                                                                          "properties": {
                                                                                            "league_name": {
                                                                                              "contains": {
                                                                                                "required": [
                                                                                                  "value"
                                                                                                ],
                                                                                                "properties": {
                                                                                                  "value": {
                                                                                                    "enum": [
                                                                                                      "wwe",
                                                                                                      "WWE",
                                                                                                      "المصارعة العالمية الترفيهية"
                                                                                                    ]
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        },
                                                                                        "else": {
                                                                                          "if": {
                                                                                            "required": [
                                                                                              "league_name"
                                                                                            ],
                                                                                            "properties": {
                                                                                              "league_name": {
                                                                                                "contains": {
                                                                                                  "required": [
                                                                                                    "value"
                                                                                                  ],
                                                                                                  "properties": {
                                                                                                    "value": {
                                                                                                      "enum": [
                                                                                                        "اتحاد كرة القدم الأميركي",
                                                                                                        "nfl",
                                                                                                        "NFL"
                                                                                                      ]
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          },
                                                                                          "else": {
                                                                                            "if": {
                                                                                              "required": [
                                                                                                "league_name"
                                                                                              ],
                                                                                              "properties": {
                                                                                                "league_name": {
                                                                                                  "contains": {
                                                                                                    "required": [
                                                                                                      "value"
                                                                                                    ],
                                                                                                    "properties": {
                                                                                                      "value": {
                                                                                                        "enum": [
                                                                                                          "ufc",
                                                                                                          "UFC",
                                                                                                          "بطولة القتال النهائي"
                                                                                                        ]
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            },
                                                                                            "else": {
                                                                                              "if": {
                                                                                                "required": [
                                                                                                  "league_name"
                                                                                                ],
                                                                                                "properties": {
                                                                                                  "league_name": {
                                                                                                    "contains": {
                                                                                                      "required": [
                                                                                                        "value"
                                                                                                      ],
                                                                                                      "properties": {
                                                                                                        "value": {
                                                                                                          "enum": [
                                                                                                            "Baloncesto japonés",
                                                                                                            "Basketball japonais",
                                                                                                            "Japanese Basketball",
                                                                                                            "日本/Bリーグ",
                                                                                                            "japanese_basketball",
                                                                                                            "Japansk basket",
                                                                                                            "Japans basketbal",
                                                                                                            "Basquete japonês",
                                                                                                            "كرة السلة اليابانية",
                                                                                                            "Japońska koszykówka",
                                                                                                            "Campionato di basket giapponese",
                                                                                                            "Japanischer Basketball"
                                                                                                          ]
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              },
                                                                                              "else": {
                                                                                                "if": {
                                                                                                  "required": [
                                                                                                    "league_name"
                                                                                                  ],
                                                                                                  "properties": {
                                                                                                    "league_name": {
                                                                                                      "contains": {
                                                                                                        "required": [
                                                                                                          "value"
                                                                                                        ],
                                                                                                        "properties": {
                                                                                                          "value": {
                                                                                                            "enum": [
                                                                                                              "wnba",
                                                                                                              "الاتحاد الوطني لكرة السلة النسائية",
                                                                                                              "WNBA"
                                                                                                            ]
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                },
                                                                                                "else": {
                                                                                                  "if": {
                                                                                                    "required": [
                                                                                                      "league_name"
                                                                                                    ],
                                                                                                    "properties": {
                                                                                                      "league_name": {
                                                                                                        "contains": {
                                                                                                          "required": [
                                                                                                            "value"
                                                                                                          ],
                                                                                                          "properties": {
                                                                                                            "value": {
                                                                                                              "enum": [
                                                                                                                "mlb",
                                                                                                                "MLB",
                                                                                                                "Ligue majeure de baseball",
                                                                                                                "دوري البيسبول الرئيسي"
                                                                                                              ]
                                                                                                            }
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  },
                                                                                                  "else": {
                                                                                                    "if": {
                                                                                                      "required": [
                                                                                                        "league_name"
                                                                                                      ],
                                                                                                      "properties": {
                                                                                                        "league_name": {
                                                                                                          "contains": {
                                                                                                            "required": [
                                                                                                              "value"
                                                                                                            ],
                                                                                                            "properties": {
                                                                                                              "value": {
                                                                                                                "enum": [
                                                                                                                  "تنس",
                                                                                                                  "Tennis",
                                                                                                                  "Tenis",
                                                                                                                  "Tênis",
                                                                                                                  "テニス",
                                                                                                                  "tennis"
                                                                                                                ]
                                                                                                              }
                                                                                                            }
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    },
                                                                                                    "then": {
                                                                                                      "properties": {
                                                                                                        "team_name": {
                                                                                                          "items": {
                                                                                                            "properties": {
                                                                                                              "value": {
                                                                                                                "enum": [
                                                                                                                  "Tennis"
                                                                                                                ]
                                                                                                              }
                                                                                                            }
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  },
                                                                                                  "then": {
                                                                                                    "properties": {
                                                                                                      "team_name": {
                                                                                                        "items": {
                                                                                                          "properties": {
                                                                                                            "value": {
                                                                                                              "enum": [
                                                                                                                "Arizona Diamondbacks",
                                                                                                                "Atlanta Braves",
                                                                                                                "Baltimore Orioles",
                                                                                                                "Boston Beaneaters",
                                                                                                                "Boston Beans",
                                                                                                                "Boston Red Sox",
                                                                                                                "California Angels",
                                                                                                                "Chicago Cubs",
                                                                                                                "Chicago White Sox",
                                                                                                                "Chicago White Stockings",
                                                                                                                "Chicago Whitesox",
                                                                                                                "Cincinnati Redlegs",
                                                                                                                "Cincinnati Reds",
                                                                                                                "Cleveland Blues",
                                                                                                                "Cleveland Indians",
                                                                                                                "Cleveland Naps",
                                                                                                                "Colorado Rockies",
                                                                                                                "Detroit Tigers",
                                                                                                                "Houston Astros",
                                                                                                                "Kansas City Athletics",
                                                                                                                "Kansas City Royals",
                                                                                                                "Los Angeles Angels",
                                                                                                                "Los Angeles Dodgers",
                                                                                                                "Miami Marlins",
                                                                                                                "Milwaukee Braves",
                                                                                                                "Milwaukee Brewers",
                                                                                                                "Minnesota Twins",
                                                                                                                "Montreal Expos",
                                                                                                                "New York Highlanders",
                                                                                                                "New York Mets",
                                                                                                                "New York Yankees",
                                                                                                                "Oakland Athletics",
                                                                                                                "Philadelphia Athletics",
                                                                                                                "Philadelphia Phillies",
                                                                                                                "Pittsburgh Pirates",
                                                                                                                "San Diego Padres",
                                                                                                                "San Francisco Giants",
                                                                                                                "Seattle Mariners",
                                                                                                                "St. Louis Cardinals",
                                                                                                                "Tampa Bay Rays",
                                                                                                                "Tampa Rays",
                                                                                                                "Texas Rangers",
                                                                                                                "Toronto Blue Jays",
                                                                                                                "Washington Nationals"
                                                                                                              ]
                                                                                                            }
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                },
                                                                                                "then": {
                                                                                                  "properties": {
                                                                                                    "team_name": {
                                                                                                      "items": {
                                                                                                        "properties": {
                                                                                                          "value": {
                                                                                                            "enum": [
                                                                                                              "Atlanta Dream",
                                                                                                              "Charlotte Sting",
                                                                                                              "Chicago Sky",
                                                                                                              "Cleveland Rockers",
                                                                                                              "Connecticut Sun",
                                                                                                              "Dallas Wings",
                                                                                                              "Detroit Shock",
                                                                                                              "Golden State Valkyries",
                                                                                                              "Houston Comets",
                                                                                                              "Indiana Fever",
                                                                                                              "Las Vegas Aces",
                                                                                                              "Los Angeles Sparks",
                                                                                                              "Miami Sol",
                                                                                                              "Minnesota Lynx",
                                                                                                              "New York Liberty",
                                                                                                              "Phoenix Mercury",
                                                                                                              "Portland Fire",
                                                                                                              "Sacramento Monarchs",
                                                                                                              "San Antonio Silver Stars",
                                                                                                              "Seattle Storm",
                                                                                                              "Toronto Tempo",
                                                                                                              "Tulsa Shock",
                                                                                                              "Washington Mystics"
                                                                                                            ]
                                                                                                          }
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              },
                                                                                              "then": {
                                                                                                "properties": {
                                                                                                  "team_name": {
                                                                                                    "items": {
                                                                                                      "properties": {
                                                                                                        "value": {
                                                                                                          "enum": [
                                                                                                            "AISIN AW AREIONS ANJO",
                                                                                                            "AKITA NORTHERN HAPPINETS",
                                                                                                            "ALVARK TOKYO",
                                                                                                            "AOMORI WAT'S",
                                                                                                            "BAMBITIOUS NARA",
                                                                                                            "CHIBA JETS",
                                                                                                            "EARTHFRIENDS TOKYO Z",
                                                                                                            "EHIME ORANGE VIKINGS",
                                                                                                            "F EAGLES NAGOYA",
                                                                                                            "FUKUSHIMA FIREBONDS",
                                                                                                            "GUNMA CRANE THUNDERS",
                                                                                                            "HIROSHIMA DRAGONFLIES",
                                                                                                            "IBARAKI ROBOTS",
                                                                                                            "IWATE BIG BULLS",
                                                                                                            "KAGAWA FIVE ARROWS",
                                                                                                            "KAGOSHIMA REBNISE",
                                                                                                            "KANAZAWA SAMURAIZ",
                                                                                                            "KAWASAKI BRAVE THUNDERS",
                                                                                                            "KUMAMOTO VOLTERS",
                                                                                                            "KYOTO HANNARYZ",
                                                                                                            "LEVANGA HOKKAIDO",
                                                                                                            "NAGOYA DIAMOND DOLPHINS",
                                                                                                            "NIIGATA ALBIREX BB",
                                                                                                            "NISHINOMIYA STORKS",
                                                                                                            "OSAKA EVESSA",
                                                                                                            "OTSUKA CORPORATION ALPHAS",
                                                                                                            "RIZING ZEPHYR FUKUOKA",
                                                                                                            "RYUKYU GOLDEN KINGS",
                                                                                                            "SAITAMA BRONCOS",
                                                                                                            "SAN-EN NEOPHOENIX",
                                                                                                            "SEAHORSES MIKAWA",
                                                                                                            "SENDAI EIGHTY NINERS",
                                                                                                            "SHIGA LAKESTARS",
                                                                                                            "SHIMANE SUSANOO MAGIC",
                                                                                                            "SHINSHU BRAVE WARRIORS",
                                                                                                            "SUNROCKERS SHIBUYA",
                                                                                                            "TOCHIGI BREX",
                                                                                                            "TOKIO MARINE NICHIDO BIG BLUE",
                                                                                                            "TOKYO CINQ REVES",
                                                                                                            "TOKYO EXCELLENCE",
                                                                                                            "TOKYO HACHIOJI TRAINS",
                                                                                                            "TOYAMA GROUSES",
                                                                                                            "TOYODA GOSEI SCORPIONS",
                                                                                                            "YAMAGATA WYVERNS",
                                                                                                            "YOKOHAMA B-CORSAIRS"
                                                                                                          ]
                                                                                                        }
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            },
                                                                                            "then": {
                                                                                              "properties": {
                                                                                                "team_name": {
                                                                                                  "items": {
                                                                                                    "properties": {
                                                                                                      "value": {
                                                                                                        "enum": [
                                                                                                          "Al Iaquinta",
                                                                                                          "Alejandro Perez",
                                                                                                          "Alex Oliveira",
                                                                                                          "Alex Perez",
                                                                                                          "Alexa Grasso",
                                                                                                          "Alexander Gustafsson",
                                                                                                          "Alexander Hernandez",
                                                                                                          "Alexander Volkanoski",
                                                                                                          "Alexander Volkov",
                                                                                                          "Alexandre Pantoja",
                                                                                                          "Alexis Davis",
                                                                                                          "Alistair Overeem",
                                                                                                          "Aljamain Sterling",
                                                                                                          "Amanda Nunes",
                                                                                                          "Andrea Lee",
                                                                                                          "Andrei Arlovski",
                                                                                                          "Angela Hill",
                                                                                                          "Anthony Pettis",
                                                                                                          "Anthony Smith",
                                                                                                          "Antonio Carlos Junior",
                                                                                                          "Ashlee Evans-Smith",
                                                                                                          "Aspen Ladd",
                                                                                                          "Ben Nguyen",
                                                                                                          "Bethe Correia",
                                                                                                          "Brad Tavares",
                                                                                                          "Brandon Moreno",
                                                                                                          "Brian Ortega",
                                                                                                          "Carla Esparza",
                                                                                                          "Cat Zingano",
                                                                                                          "Chad Mendes",
                                                                                                          "Chan Sung Jung",
                                                                                                          "Chris Weidman",
                                                                                                          "Claudia Gadelha",
                                                                                                          "Cody Garbrandt",
                                                                                                          "Cody Stamann",
                                                                                                          "Colby Covington",
                                                                                                          "Conor McGregor",
                                                                                                          "Corey Anderson",
                                                                                                          "Cortney Casey",
                                                                                                          "Cris Cyborg",
                                                                                                          "Cub Swanson",
                                                                                                          "Curtis Blaydes",
                                                                                                          "Dan Hooker",
                                                                                                          "Daniel Cormier",
                                                                                                          "Darren Elkins",
                                                                                                          "Darren Till",
                                                                                                          "David Branch",
                                                                                                          "Deiveson Figueiredo",
                                                                                                          "Demian Maia",
                                                                                                          "Derek Brunson",
                                                                                                          "Derrick Lewis",
                                                                                                          "Dominick Cruz",
                                                                                                          "Dominick Reyes",
                                                                                                          "Donald Cerrone",
                                                                                                          "Douglas Silva de Andrade",
                                                                                                          "Dustin Ortiz",
                                                                                                          "Dustin Poirier",
                                                                                                          "Edson Barboza",
                                                                                                          "Elias Theodorou",
                                                                                                          "Elizeu Zaleski dos Santos",
                                                                                                          "Felice Herrig",
                                                                                                          "Francis Ngannou",
                                                                                                          "Francisco Trinaldo",
                                                                                                          "Frankie Edgar",
                                                                                                          "Georges St-Pierre",
                                                                                                          "Germaine de Randamie",
                                                                                                          "Glover Teixeira",
                                                                                                          "Gunnar Nelson",
                                                                                                          "Henry Cejudo",
                                                                                                          "Holly Holm",
                                                                                                          "Ilir Latifi",
                                                                                                          "Irene Aldana",
                                                                                                          "Israel Adesanya",
                                                                                                          "Jacare Souza",
                                                                                                          "James Vick",
                                                                                                          "Jan Blachowicz",
                                                                                                          "Jared Cannonier",
                                                                                                          "Jennifer Maia",
                                                                                                          "Jeremy Stephens",
                                                                                                          "Jessica Andrade",
                                                                                                          "Jessica Eye",
                                                                                                          "Jessica-Rose Clark",
                                                                                                          "Jimi Manuwa",
                                                                                                          "Jimmie Rivera",
                                                                                                          "Joanna Jedrzejczyk",
                                                                                                          "Joanne Calderwood",
                                                                                                          "John Dodson",
                                                                                                          "John Lineker",
                                                                                                          "John Moraga",
                                                                                                          "Jon Jones",
                                                                                                          "Jorge Masvidal",
                                                                                                          "Jose Aldo",
                                                                                                          "Joseph Benavidez",
                                                                                                          "Josh Emmett",
                                                                                                          "Julianna Pena",
                                                                                                          "Junior dos Santos",
                                                                                                          "Jussier Formiga",
                                                                                                          "Justin Gaethje",
                                                                                                          "Justin Willis",
                                                                                                          "Kamaru Usman",
                                                                                                          "Karolina Kowalkiewicz",
                                                                                                          "Katlyn Chookagian",
                                                                                                          "Kelvin Gastelum",
                                                                                                          "Ketlen Vieira",
                                                                                                          "Kevin Lee",
                                                                                                          "Khabib Nurmagomedov",
                                                                                                          "Lauren Murphy Increase1",
                                                                                                          "Leon Edwards",
                                                                                                          "Lina Lansberg",
                                                                                                          "Liz Carmouche",
                                                                                                          "Lucie Pudilova",
                                                                                                          "Luke Rockhold",
                                                                                                          "Mackenzie Dern",
                                                                                                          "Mara Romero Borella",
                                                                                                          "Marcin Tybura",
                                                                                                          "Marion Reneau",
                                                                                                          "Mark Hunt",
                                                                                                          "Marlon Moraes",
                                                                                                          "Matheus Nicolau",
                                                                                                          "Mauricio Rua",
                                                                                                          "Max Holloway",
                                                                                                          "Michael Chiesa",
                                                                                                          "Michelle Waterson",
                                                                                                          "Middleweight",
                                                                                                          "Mirsad Bektic",
                                                                                                          "Misha Cirkunov",
                                                                                                          "Nate Diaz",
                                                                                                          "Neil Magny",
                                                                                                          "Nicco Montaño",
                                                                                                          "Nikita Krylov",
                                                                                                          "Nina Ansaroff",
                                                                                                          "Oleksiy Oliynyk",
                                                                                                          "Ovince Saint Preux",
                                                                                                          "Paul Felder",
                                                                                                          "Paulo Costa",
                                                                                                          "Pedro Munhoz",
                                                                                                          "Rafael dos Anjos",
                                                                                                          "Randa Markos",
                                                                                                          "Rani Yahya",
                                                                                                          "Raphael Assunção",
                                                                                                          "Raquel Pennington",
                                                                                                          "Ray Borg",
                                                                                                          "Renato Moicano",
                                                                                                          "Ricardo Lamas",
                                                                                                          "Rob Font",
                                                                                                          "Robbie Lawler",
                                                                                                          "Robert Whittaker",
                                                                                                          "Rose Namajunas",
                                                                                                          "Roxanne Modafferi",
                                                                                                          "Santiago Ponzinibbio",
                                                                                                          "Sara McMann",
                                                                                                          "Sergio Pettis",
                                                                                                          "Shamil Abdurakhimov",
                                                                                                          "Sijara Eubanks",
                                                                                                          "Stefan Struve",
                                                                                                          "Stephen Thompson",
                                                                                                          "Stipe Miocic",
                                                                                                          "Tai Tuivasa",
                                                                                                          "Tatiana Suarez",
                                                                                                          "Tecia Torres",
                                                                                                          "Thiago Santos",
                                                                                                          "Thomas Almeida",
                                                                                                          "Tim Elliott",
                                                                                                          "TJ Dillashaw",
                                                                                                          "Tony Ferguson",
                                                                                                          "Tonya Evinger",
                                                                                                          "Tyron Woodley",
                                                                                                          "Tyson Pedro",
                                                                                                          "Ulka Sasaki",
                                                                                                          "Uriah Hall",
                                                                                                          "Valentina Shevchenko",
                                                                                                          "Volkan Oezdemir",
                                                                                                          "Wilson Reis",
                                                                                                          "Yair Rodriguez",
                                                                                                          "Yana Kunitskaya",
                                                                                                          "Yoel Romero",
                                                                                                          "Zabit Magomedsharipov"
                                                                                                        ]
                                                                                                      }
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          },
                                                                                          "then": {
                                                                                            "properties": {
                                                                                              "team_name": {
                                                                                                "items": {
                                                                                                  "properties": {
                                                                                                    "value": {
                                                                                                      "enum": [
                                                                                                        "Arizona Cardinals",
                                                                                                        "Atlanta Falcons",
                                                                                                        "Baltimore Ravens",
                                                                                                        "Boston Patriots",
                                                                                                        "Boston Redskins",
                                                                                                        "Buffalo Bills",
                                                                                                        "Carolina Panthers",
                                                                                                        "Chicago Bears",
                                                                                                        "Chicago Cardinals",
                                                                                                        "Cincinnati Bengals",
                                                                                                        "Cleveland Browns",
                                                                                                        "Dallas Cowboys",
                                                                                                        "Dallas Texans",
                                                                                                        "Denver Broncos",
                                                                                                        "Detroit Lions",
                                                                                                        "Green Bay Packers",
                                                                                                        "Houston Oilers",
                                                                                                        "Houston Texans",
                                                                                                        "Indianapolis Colts",
                                                                                                        "Jacksonville Jaguars",
                                                                                                        "Kansas City Chiefs",
                                                                                                        "Las Vegas Raiders",
                                                                                                        "Los Angeles Chargers",
                                                                                                        "Los Angeles Rams",
                                                                                                        "Miami Dolphins",
                                                                                                        "Minnesota Vikings",
                                                                                                        "New England Patriots",
                                                                                                        "New Orleans Saints",
                                                                                                        "New York Giants",
                                                                                                        "New York Jets",
                                                                                                        "New York Titans",
                                                                                                        "Oakland Raiders",
                                                                                                        "Philadelphia Eagles",
                                                                                                        "Pittsburgh Steelers",
                                                                                                        "San Diego Chargers",
                                                                                                        "San Francisco 49ers",
                                                                                                        "Seattle Seahawks",
                                                                                                        "St. Louis Rams",
                                                                                                        "Tampa Bay Buccaneers",
                                                                                                        "Tennessee Titans",
                                                                                                        "Washington Commanders",
                                                                                                        "Washington Football Team"
                                                                                                      ]
                                                                                                    }
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        },
                                                                                        "then": {
                                                                                          "properties": {
                                                                                            "team_name": {
                                                                                              "items": {
                                                                                                "properties": {
                                                                                                  "value": {
                                                                                                    "enum": [
                                                                                                      "WWE"
                                                                                                    ]
                                                                                                  }
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      },
                                                                                      "then": {
                                                                                        "properties": {
                                                                                          "team_name": {
                                                                                            "items": {
                                                                                              "properties": {
                                                                                                "value": {
                                                                                                  "enum": [
                                                                                                    "Chennai Super Kings",
                                                                                                    "Delhi Capitals",
                                                                                                    "Gujarat Lions",
                                                                                                    "Kings XI Punjab",
                                                                                                    "Kolkata Knight Riders",
                                                                                                    "Mumbai Indians",
                                                                                                    "Rajasthan Royals",
                                                                                                    "Rising Pune Supergiants",
                                                                                                    "Royal Challengers Bangalore",
                                                                                                    "Sunrisers Hyderabad"
                                                                                                  ]
                                                                                                }
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    },
                                                                                    "then": {
                                                                                      "properties": {
                                                                                        "team_name": {
                                                                                          "items": {
                                                                                            "properties": {
                                                                                              "value": {
                                                                                                "enum": [
                                                                                                  "Team Cuba",
                                                                                                  "Team Dominican Republic",
                                                                                                  "Team Japan",
                                                                                                  "Team Netherlands",
                                                                                                  "Team Panama",
                                                                                                  "Team Puerto Rico",
                                                                                                  "Team South Korea",
                                                                                                  "Team United States",
                                                                                                  "Team Venezuela"
                                                                                                ]
                                                                                              }
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  },
                                                                                  "then": {
                                                                                    "properties": {
                                                                                      "team_name": {
                                                                                        "items": {
                                                                                          "properties": {
                                                                                            "value": {
                                                                                              "enum": [
                                                                                                "AC Nagano Parceiro",
                                                                                                "Albirex Niigata",
                                                                                                "Avispa Fukuoka",
                                                                                                "Blaublitz Akita",
                                                                                                "Cerezo Osaka",
                                                                                                "Consadole Sapporo",
                                                                                                "Ehime FC",
                                                                                                "F.C. Gifu",
                                                                                                "Fagiano Okayama FC",
                                                                                                "FC Machida Zelvia",
                                                                                                "FC Ryūkyū",
                                                                                                "FC Tokyo",
                                                                                                "Fujieda MYFC",
                                                                                                "Fukushima United FC",
                                                                                                "Gainare Tottori",
                                                                                                "Gamba Osaka",
                                                                                                "Giravanz Kitakyushu",
                                                                                                "Grulla Morioka",
                                                                                                "Iwaki FC",
                                                                                                "JEF United Ichihara Chiba",
                                                                                                "Júbilo Iwata",
                                                                                                "Kamatamare Sanuki",
                                                                                                "Kashima Antlers",
                                                                                                "Kashiwa Reysol",
                                                                                                "Kataller Toyama",
                                                                                                "Kawasaki Frontale",
                                                                                                "Kyoto Sanga FC",
                                                                                                "Matsumoto Yamaga FC",
                                                                                                "Mito HollyHock",
                                                                                                "Montedio Yamagata",
                                                                                                "Nagoya Grampus Eight",
                                                                                                "Oita Trinita",
                                                                                                "Omiya Ardija",
                                                                                                "RENOFA Yamaguchi",
                                                                                                "Roasso Kumamoto",
                                                                                                "Sagan Tosu",
                                                                                                "Sanfrecce Hiroshima",
                                                                                                "SC Sagamihara",
                                                                                                "Shimizu S-Pulse",
                                                                                                "Shonan Bellmare",
                                                                                                "Thespakusatsu Gunma",
                                                                                                "Tochigi SC",
                                                                                                "Tokushima Vortis",
                                                                                                "Tokyo Verdy1969",
                                                                                                "Urawa Red Diamonds",
                                                                                                "V-Varen Nagasaki",
                                                                                                "Vegalta Sendai",
                                                                                                "Ventforet Kofu",
                                                                                                "Vissel Kobe",
                                                                                                "Yokohama F. Marinos",
                                                                                                "Yokohama FC",
                                                                                                "YSCC Yokohama",
                                                                                                "Zweigen Kanazawa"
                                                                                              ]
                                                                                            }
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                },
                                                                                "then": {
                                                                                  "properties": {
                                                                                    "team_name": {
                                                                                      "items": {
                                                                                        "properties": {
                                                                                          "value": {
                                                                                            "enum": [
                                                                                              "Ahmedabad Defenders",
                                                                                              "Black Hawks Hyderabad",
                                                                                              "Calicut Heroes",
                                                                                              "Chennai Spartans",
                                                                                              "Kochi Blue Spikers",
                                                                                              "U Mumba Volley"
                                                                                            ]
                                                                                          }
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                }
                                                                              },
                                                                              "then": {
                                                                                "properties": {
                                                                                  "team_name": {
                                                                                    "items": {
                                                                                      "properties": {
                                                                                        "value": {
                                                                                          "enum": [
                                                                                            "A.S. Livorno Calcio",
                                                                                            "AC Milan",
                                                                                            "Ascoli",
                                                                                            "Atalanta",
                                                                                            "Bari",
                                                                                            "Bologna",
                                                                                            "Brescia",
                                                                                            "Cagliari Calcio",
                                                                                            "Calcio Catania",
                                                                                            "Catanzaro",
                                                                                            "Chievo Verona",
                                                                                            "Cittadella",
                                                                                            "Como",
                                                                                            "Cosenza",
                                                                                            "Empoli",
                                                                                            "Fiorentina",
                                                                                            "Frosinone FC",
                                                                                            "Genoa",
                                                                                            "Inter Milan",
                                                                                            "Juventus",
                                                                                            "Lazio",
                                                                                            "Lecce",
                                                                                            "Lecco",
                                                                                            "Modena",
                                                                                            "Monza",
                                                                                            "Palermo",
                                                                                            "Parma",
                                                                                            "Parma Calcio",
                                                                                            "Perugia",
                                                                                            "Piacenza",
                                                                                            "Pisa",
                                                                                            "Reggina",
                                                                                            "Roma",
                                                                                            "Sampdoria",
                                                                                            "Sassuolo",
                                                                                            "Spal",
                                                                                            "SSC Napoli",
                                                                                            "Ternana",
                                                                                            "Torino",
                                                                                            "Udinese",
                                                                                            "US Salernitana",
                                                                                            "Venezia FC",
                                                                                            "Verona FC"
                                                                                          ]
                                                                                        }
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                }
                                                                              }
                                                                            },
                                                                            "then": {
                                                                              "properties": {
                                                                                "team_name": {
                                                                                  "items": {
                                                                                    "properties": {
                                                                                      "value": {
                                                                                        "enum": [
                                                                                          "Dabang Mumbai HC",
                                                                                          "Delhi Waveriders",
                                                                                          "Jaypee Punjab Warriors",
                                                                                          "Kalinga Lancers",
                                                                                          "Ranchi Rays",
                                                                                          "Uttar Pradesh Wizards"
                                                                                        ]
                                                                                      }
                                                                                    }
                                                                                  }
                                                                                }
                                                                              }
                                                                            }
                                                                          },
                                                                          "then": {
                                                                            "properties": {
                                                                              "team_name": {
                                                                                "items": {
                                                                                  "properties": {
                                                                                    "value": {
                                                                                      "enum": [
                                                                                        "Buffalo Bandits",
                                                                                        "Calgary Roughnecks",
                                                                                        "Colorado Mammoth",
                                                                                        "Georgia Swarm",
                                                                                        "Halifax Thunderbirds",
                                                                                        "New England Black Wolves",
                                                                                        "New York Riptide",
                                                                                        "Philadelphia Wings",
                                                                                        "Rochester Knighthawks",
                                                                                        "San Diego Seals",
                                                                                        "Saskatchewan Rush",
                                                                                        "Toronto Rock",
                                                                                        "Vancouver Warriors"
                                                                                      ]
                                                                                    }
                                                                                  }
                                                                                }
                                                                              }
                                                                            }
                                                                          }
                                                                        },
                                                                        "then": {
                                                                          "properties": {
                                                                            "team_name": {
                                                                              "items": {
                                                                                "properties": {
                                                                                  "value": {
                                                                                    "enum": [
                                                                                      "Afghanistan",
                                                                                      "Australia",
                                                                                      "Bangladesh",
                                                                                      "England",
                                                                                      "India",
                                                                                      "Ireland",
                                                                                      "New Zealand",
                                                                                      "Pakistan",
                                                                                      "South Africa",
                                                                                      "Sri Lanka",
                                                                                      "West Indies",
                                                                                      "Zimbabwe"
                                                                                    ]
                                                                                  }
                                                                                }
                                                                              }
                                                                            }
                                                                          }
                                                                        }
                                                                      },
                                                                      "then": {
                                                                        "properties": {
                                                                          "team_name": {
                                                                            "items": {
                                                                              "properties": {
                                                                                "value": {
                                                                                  "enum": [
                                                                                    "LPGA"
                                                                                  ]
                                                                                }
                                                                              }
                                                                            }
                                                                          }
                                                                        }
                                                                      }
                                                                    },
                                                                    "then": {
                                                                      "properties": {
                                                                        "team_name": {
                                                                          "items": {
                                                                            "properties": {
                                                                              "value": {
                                                                                "enum": [
                                                                                  "AC Ajaccio",
                                                                                  "Amiens SC",
                                                                                  "Angers SCO",
                                                                                  "AS Saint-Etienne",
                                                                                  "Auxerre",
                                                                                  "Bastia",
                                                                                  "Bordeaux",
                                                                                  "Brest",
                                                                                  "Clermont Foot 63",
                                                                                  "Dijon FCO",
                                                                                  "FC Lorient",
                                                                                  "Guingamp",
                                                                                  "Le Havre",
                                                                                  "Lens",
                                                                                  "Lille",
                                                                                  "Lyon",
                                                                                  "Marseille",
                                                                                  "Metz",
                                                                                  "Monaco",
                                                                                  "Montpellier",
                                                                                  "Nantes",
                                                                                  "Nice",
                                                                                  "Nîmes Olympique",
                                                                                  "PSG",
                                                                                  "Rennes",
                                                                                  "Sedan",
                                                                                  "SM Caen",
                                                                                  "Sochaux",
                                                                                  "Stade de Reims",
                                                                                  "Strasbourg",
                                                                                  "Thonon Evian FC",
                                                                                  "Toulouse FC",
                                                                                  "Troyes",
                                                                                  "Valenciennes FC"
                                                                                ]
                                                                              }
                                                                            }
                                                                          }
                                                                        }
                                                                      }
                                                                    }
                                                                  },
                                                                  "then": {
                                                                    "properties": {
                                                                      "team_name": {
                                                                        "items": {
                                                                          "properties": {
                                                                            "value": {
                                                                              "enum": [
                                                                                "Aberdeen",
                                                                                "Airdrieonians",
                                                                                "Arbroath",
                                                                                "Celtic",
                                                                                "Dundee",
                                                                                "Dundee United",
                                                                                "Dunfermline",
                                                                                "Hearts",
                                                                                "Hibernian",
                                                                                "Inverness Caledonian Thistle",
                                                                                "Kilmarnock",
                                                                                "Livingston",
                                                                                "Motherwell",
                                                                                "Patrick Thistle",
                                                                                "Rangers",
                                                                                "Ross County",
                                                                                "St Johnstone",
                                                                                "St Mirren"
                                                                              ]
                                                                            }
                                                                          }
                                                                        }
                                                                      }
                                                                    }
                                                                  }
                                                                },
                                                                "then": {
                                                                  "properties": {
                                                                    "team_name": {
                                                                      "items": {
                                                                        "properties": {
                                                                          "value": {
                                                                            "enum": [
                                                                              "PGA"
                                                                            ]
                                                                          }
                                                                        }
                                                                      }
                                                                    }
                                                                  }
                                                                }
                                                              },
                                                              "then": {
                                                                "properties": {
                                                                  "team_name": {
                                                                    "items": {
                                                                      "properties": {
                                                                        "value": {
                                                                          "enum": [
                                                                            "Bengal Warriors",
                                                                            "Bengaluru Bulls",
                                                                            "Dabang Delhi KC",
                                                                            "Gujarat Fortunegiants",
                                                                            "Haryana Steelers",
                                                                            "Jaipur Pink Panthers",
                                                                            "Patna Pirates",
                                                                            "Puneri Paltan",
                                                                            "Tamil Thalaivas",
                                                                            "Telugu Titans",
                                                                            "U Mumba",
                                                                            "UP Yoddha"
                                                                          ]
                                                                        }
                                                                      }
                                                                    }
                                                                  }
                                                                }
                                                              }
                                                            },
                                                            "then": {
                                                              "properties": {
                                                                "team_name": {
                                                                  "items": {
                                                                    "properties": {
                                                                      "value": {
                                                                        "enum": [
                                                                          "Angel City FC",
                                                                          "Boston Legacy FC",
                                                                          "Chicago Red Stars",
                                                                          "Houston Dash",
                                                                          "Kansas City Current",
                                                                          "NJ/NY Gotham FC",
                                                                          "North Carolina Courage",
                                                                          "Orlando Pride",
                                                                          "Portland Thorns FC",
                                                                          "Racing Louisville FC",
                                                                          "San Diego Wave FC",
                                                                          "Seattle Reign FC",
                                                                          "Sky Blue FC",
                                                                          "Utah Royals FC",
                                                                          "Washington Spirit"
                                                                        ]
                                                                      }
                                                                    }
                                                                  }
                                                                }
                                                              }
                                                            }
                                                          },
                                                          "then": {
                                                            "properties": {
                                                              "team_name": {
                                                                "items": {
                                                                  "properties": {
                                                                    "value": {
                                                                      "enum": [
                                                                        "1. FC Koln",
                                                                        "1. FC Magdeburg",
                                                                        "Arminia Bielefeld",
                                                                        "Bayer Leverkusen",
                                                                        "Bayern Munich",
                                                                        "Borussia Dortmund",
                                                                        "Borussia Monchengladbach",
                                                                        "Darmstadt 98",
                                                                        "Dynamo Dresden",
                                                                        "Eintracht Braunschweig",
                                                                        "Eintracht Frankfurt",
                                                                        "Energie Cottbus",
                                                                        "FC Augsburg",
                                                                        "FC Heidenheim",
                                                                        "FC St. Pauli",
                                                                        "Fortuna Düsseldorf",
                                                                        "FSV Mainz 05",
                                                                        "Greuther Fürth",
                                                                        "Hamburg SV",
                                                                        "Hannover 96",
                                                                        "Hansa Rostock",
                                                                        "Hertha Berlin",
                                                                        "Hertha BSC",
                                                                        "Kaiserslautern",
                                                                        "Karlsruher SC",
                                                                        "Nurnberg",
                                                                        "RB Leipzig",
                                                                        "Schalke",
                                                                        "Sport-Club Freiburg",
                                                                        "TSG 1899 Hoffenheim",
                                                                        "TSV 1860 Munich",
                                                                        "Union Berlin",
                                                                        "VfB Stuttgart",
                                                                        "VfL Bochum",
                                                                        "VfL Osnabrück",
                                                                        "VfL Wolfsburg",
                                                                        "Werder Bremen"
                                                                      ]
                                                                    }
                                                                  }
                                                                }
                                                              }
                                                            }
                                                          }
                                                        },
                                                        "then": {
                                                          "properties": {
                                                            "team_name": {
                                                              "items": {
                                                                "properties": {
                                                                  "value": {
                                                                    "enum": [
                                                                      "X-Games"
                                                                    ]
                                                                  }
                                                                }
                                                              }
                                                            }
                                                          }
                                                        }
                                                      },
                                                      "then": {
                                                        "properties": {
                                                          "team_name": {
                                                            "items": {
                                                              "properties": {
                                                                "value": {
                                                                  "enum": [
                                                                    "ADO Den Haag",
                                                                    "Ajax Amsterdam",
                                                                    "Almere City",
                                                                    "AZ Alkmaar",
                                                                    "De Graafschap",
                                                                    "Excelsior",
                                                                    "FC Groningen",
                                                                    "FC Utrecht",
                                                                    "FC Volendam",
                                                                    "FC Zwolle",
                                                                    "Feyenoord Rotterdam",
                                                                    "Fortuna Sittard",
                                                                    "Go Ahead Eagles",
                                                                    "Heerenveen",
                                                                    "Heracles Almelo",
                                                                    "NAC Breda",
                                                                    "NEC Nijmegen",
                                                                    "PSV Eindhoven",
                                                                    "RBC Roosendaal",
                                                                    "RKC Waalwijk",
                                                                    "Roda JC Kerkrade",
                                                                    "SC Cambuur",
                                                                    "Sparta Rotterdam",
                                                                    "Twente Enschede",
                                                                    "Vitesse Arnhem",
                                                                    "Willem II Tilburg"
                                                                  ]
                                                                }
                                                              }
                                                            }
                                                          }
                                                        }
                                                      }
                                                    },
                                                    "then": {
                                                      "properties": {
                                                        "team_name": {
                                                          "items": {
                                                            "properties": {
                                                              "value": {
                                                                "enum": [
                                                                  "Atlético de San Luis",
                                                                  "CF Atlas",
                                                                  "CF Monterrey",
                                                                  "Club América",
                                                                  "Club Deportivo Guadalajara - Chivas",
                                                                  "Club Deportivo Social y Cultural - Cruz Azul",
                                                                  "Club Santos Laguna",
                                                                  "Club Universidad Nacional A.C. - Pumas",
                                                                  "FC Juárez",
                                                                  "Mazatlán",
                                                                  "Necaxa",
                                                                  "Querétaro",
                                                                  "UANL Tigres"
                                                                ]
                                                              }
                                                            }
                                                          }
                                                        }
                                                      }
                                                    }
                                                  },
                                                  "then": {
                                                    "properties": {
                                                      "team_name": {
                                                        "items": {
                                                          "properties": {
                                                            "value": {
                                                              "enum": [
                                                                "Afghanistan",
                                                                "Albania",
                                                                "Algeria",
                                                                "American Samoa",
                                                                "Andorra",
                                                                "Angola",
                                                                "Antigua and Barbuda",
                                                                "Argentina",
                                                                "Armenia",
                                                                "Aruba",
                                                                "Australia",
                                                                "Austria",
                                                                "Azerbaijan",
                                                                "Bahamas",
                                                                "Bahrain",
                                                                "Bangladesh",
                                                                "Barbados",
                                                                "Belarus",
                                                                "Belgium",
                                                                "Belize",
                                                                "Benin",
                                                                "Bermuda",
                                                                "Bhutan",
                                                                "Bolivia",
                                                                "Bosnia and Herzegovina",
                                                                "Botswana",
                                                                "Brazil",
                                                                "British Virgin Islands",
                                                                "Brunei",
                                                                "Bulgaria",
                                                                "Burkina Faso",
                                                                "Burundi",
                                                                "Cambodia",
                                                                "Cameroon",
                                                                "Canada",
                                                                "Cape Verde",
                                                                "Cayman Islands",
                                                                "Central African Republic",
                                                                "Chad",
                                                                "Chile",
                                                                "China",
                                                                "Chinese Taipei",
                                                                "Colombia",
                                                                "Comoros",
                                                                "Congo",
                                                                "Cook Islands",
                                                                "Costa Rica",
                                                                "Croatia",
                                                                "Cuba",
                                                                "Cyprus",
                                                                "Czech Republic",
                                                                "Democratic Republic of the Congo",
                                                                "Denmark",
                                                                "Djibouti",
                                                                "Dominica",
                                                                "Dominican Republic",
                                                                "East Timor",
                                                                "Ecuador",
                                                                "Egypt",
                                                                "El Salvador",
                                                                "Equatorial Guinea",
                                                                "Eritrea",
                                                                "Estonia",
                                                                "Ethiopia",
                                                                "Federated States of Micronesia",
                                                                "Fiji",
                                                                "Finland",
                                                                "France",
                                                                "Gabon",
                                                                "Georgia",
                                                                "Germany",
                                                                "Ghana",
                                                                "Great Britain",
                                                                "Greece",
                                                                "Grenada",
                                                                "Guam",
                                                                "Guatemala",
                                                                "Guinea",
                                                                "Guinea-Bissau",
                                                                "Guyana",
                                                                "Haiti",
                                                                "Honduras",
                                                                "Hong Kong",
                                                                "Hungary",
                                                                "Iceland",
                                                                "Independent Olympic Athletes",
                                                                "India",
                                                                "Indonesia",
                                                                "Iran",
                                                                "Iraq",
                                                                "Ireland",
                                                                "Israel",
                                                                "Italy",
                                                                "Ivory Coast",
                                                                "Jamaica",
                                                                "Japan",
                                                                "Jordan",
                                                                "Kazakhstan",
                                                                "Kenya",
                                                                "Kiribati",
                                                                "Kosovo",
                                                                "Kyrgyzstan",
                                                                "Laos",
                                                                "Latvia",
                                                                "Lebanon",
                                                                "Lesotho",
                                                                "Liberia",
                                                                "Libya",
                                                                "Liechtenstein",
                                                                "Lithuania",
                                                                "Luxembourg",
                                                                "Macedonia",
                                                                "Madagascar",
                                                                "Malawi",
                                                                "Malaysia",
                                                                "Maldives",
                                                                "Mali",
                                                                "Malta",
                                                                "Marshall Islands",
                                                                "Mauritania",
                                                                "Mauritius",
                                                                "Mexico",
                                                                "Moldova",
                                                                "Monaco",
                                                                "Mongolia",
                                                                "Montenegro",
                                                                "Morocco",
                                                                "Mozambique",
                                                                "Myanmar",
                                                                "Namibia",
                                                                "Nauru",
                                                                "Nepal",
                                                                "Netherlands",
                                                                "New Zealand",
                                                                "Nicaragua",
                                                                "Niger",
                                                                "Nigeria",
                                                                "North Korea",
                                                                "Norway",
                                                                "Oman",
                                                                "Pakistan",
                                                                "Palau",
                                                                "Palestine",
                                                                "Panama",
                                                                "Papua New Guinea",
                                                                "Paraguay",
                                                                "Peru",
                                                                "Philippines",
                                                                "Poland",
                                                                "Portugal",
                                                                "Puerto Rico",
                                                                "Qatar",
                                                                "Refugee Olympic Team",
                                                                "Romania",
                                                                "Russia",
                                                                "Rwanda",
                                                                "Saint Kitts and Nevis",
                                                                "Saint Lucia",
                                                                "Saint Vincent and the Grenadines",
                                                                "Samoa",
                                                                "San Marino",
                                                                "Saudi Arabia",
                                                                "Senegal",
                                                                "Serbia",
                                                                "Seychelles",
                                                                "Sierra Leone",
                                                                "Singapore",
                                                                "Slovakia",
                                                                "Slovenia",
                                                                "Solomon Islands",
                                                                "Somalia",
                                                                "South Africa",
                                                                "South Korea",
                                                                "South Sudan",
                                                                "Spain",
                                                                "Sri Lanka",
                                                                "Sudan",
                                                                "Suriname",
                                                                "Swaziland",
                                                                "Sweden",
                                                                "Switzerland",
                                                                "Syria",
                                                                "São Tomé and Príncipe",
                                                                "Tajikistan",
                                                                "Tanzania",
                                                                "Thailand",
                                                                "The Gambia",
                                                                "Togo",
                                                                "Tonga",
                                                                "Trinidad and Tobago",
                                                                "Tunisia",
                                                                "Turkey",
                                                                "Turkmenistan",
                                                                "Tuvalu",
                                                                "Uganda",
                                                                "Ukraine",
                                                                "United Arab Emirates",
                                                                "United States",
                                                                "Uruguay",
                                                                "Uzbekistan",
                                                                "Vanuatu",
                                                                "Venezuela",
                                                                "Vietnam",
                                                                "Virgin Islands",
                                                                "Yemen",
                                                                "Zambia",
                                                                "Zimbabwe"
                                                              ]
                                                            }
                                                          }
                                                        }
                                                      }
                                                    }
                                                  }
                                                },
                                                "then": {
                                                  "properties": {
                                                    "team_name": {
                                                      "items": {
                                                        "properties": {
                                                          "value": {
                                                            "enum": [
                                                              "ATK Mohun Bagan FC",
                                                              "Bengaluru FC",
                                                              "Chennaiyin FC",
                                                              "FC Goa",
                                                              "Hyderabad FC",
                                                              "Jamshedpur FC",
                                                              "Kerala Blasters FC",
                                                              "Mumbai City FC",
                                                              "Northeast United FC",
                                                              "Odisha FC"
                                                            ]
                                                          }
                                                        }
                                                      }
                                                    }
                                                  }
                                                }
                                              },
                                              "then": {
                                                "properties": {
                                                  "team_name": {
                                                    "items": {
                                                      "properties": {
                                                        "value": {
                                                          "enum": [
                                                            "Angola",
                                                            "Argentina",
                                                            "Australia",
                                                            "Austria",
                                                            "Belgium",
                                                            "Bolivia",
                                                            "Brazil",
                                                            "Bulgaria",
                                                            "Cameroon",
                                                            "Canada",
                                                            "Chile",
                                                            "China",
                                                            "Colombia",
                                                            "Costa Rica",
                                                            "Cote d'Ivoire",
                                                            "Croatia",
                                                            "Czech Republic",
                                                            "Denmark",
                                                            "Ecuador",
                                                            "England",
                                                            "France",
                                                            "Germany",
                                                            "Ghana",
                                                            "Greece",
                                                            "Iran",
                                                            "Ireland",
                                                            "Italy",
                                                            "Jamaica",
                                                            "Japan",
                                                            "Mexico",
                                                            "Morocco",
                                                            "Netherlands",
                                                            "Nigeria",
                                                            "Norway",
                                                            "Paraguay",
                                                            "Poland",
                                                            "Portugal",
                                                            "Qatar",
                                                            "Romania",
                                                            "Russia",
                                                            "Saudi Arabia",
                                                            "Scotland",
                                                            "Senegal",
                                                            "Serbia and Montenegro",
                                                            "Slovenia",
                                                            "South Africa",
                                                            "South Korea",
                                                            "Spain",
                                                            "Sweden",
                                                            "Switzerland",
                                                            "Togo",
                                                            "Trinidad and Tobago",
                                                            "Tunisia",
                                                            "Turkey",
                                                            "Ukraine",
                                                            "United States",
                                                            "Uruguay",
                                                            "Venezuela",
                                                            "Wales",
                                                            "Yugoslavia"
                                                          ]
                                                        }
                                                      }
                                                    }
                                                  }
                                                }
                                              }
                                            },
                                            "then": {
                                              "properties": {
                                                "team_name": {
                                                  "items": {
                                                    "properties": {
                                                      "value": {
                                                        "enum": [
                                                          "Abilene Christian Wildcats",
                                                          "Air Force Falcons",
                                                          "Akron Zips",
                                                          "Alabama A&M Bulldogs",
                                                          "Alabama Birmingham Blazers",
                                                          "Alabama Crimson Tide",
                                                          "Alabama State Hornets",
                                                          "Albany Great Danes",
                                                          "Alcorn State Braves",
                                                          "American University Eagles",
                                                          "Appalachian State Mountaineers",
                                                          "Arizona State Sun Devils",
                                                          "Arizona Wildcats",
                                                          "Arkansas Little Rock Trojans",
                                                          "Arkansas Razorbacks",
                                                          "Arkansas State Indians",
                                                          "Arkansas State Red Wolves",
                                                          "Arkansas-Pine Bluff Golden Lions",
                                                          "Army Black Knights",
                                                          "Auburn Tigers",
                                                          "Austin Peay Governors",
                                                          "Ball State Cardinals",
                                                          "Bates Bobcats",
                                                          "Baylor Bears",
                                                          "Belmont Bruins",
                                                          "Bethune Cookman Wildcats",
                                                          "Binghamton Bearcats",
                                                          "Boise State Broncos",
                                                          "Boston College Eagles",
                                                          "Boston University Terriers",
                                                          "Bowling Green Falcons",
                                                          "Bradley Braves",
                                                          "Brown Bears",
                                                          "Bryant Bulldogs",
                                                          "Bucknell Bison",
                                                          "Buffalo Bulls",
                                                          "Butler Bulldogs",
                                                          "BYU Cougars",
                                                          "Cal Irvine Anteaters",
                                                          "Cal Poly Mustangs",
                                                          "Cal Riverside Highlanders",
                                                          "Cal Santa Barbara Gauchos",
                                                          "Cal State Bakersfield Roadrunners",
                                                          "Cal State Fullerton Titans",
                                                          "Cal State Northridge Matadors",
                                                          "Cal State Sacramento Hornets",
                                                          "California Baptist Lancers",
                                                          "California Golden Bears",
                                                          "Campbell Fighting Camels",
                                                          "Canisius Golden Griffins",
                                                          "Centenary Gentlemen",
                                                          "Central Arkansas Bears",
                                                          "Central Connecticut Blue Devils",
                                                          "Central Connecticut State Blue Devils",
                                                          "Central Florida Golden Knights",
                                                          "Central Michigan Chippewas",
                                                          "Charleston Cougars",
                                                          "Charleston Southern Buccaneers",
                                                          "Charlotte 49ers",
                                                          "Chicago State Cougars",
                                                          "Cincinnati Bearcats",
                                                          "Citadel Bulldogs",
                                                          "Clemson Tigers",
                                                          "Cleveland State Vikings",
                                                          "Coastal Carolina Chanticleers",
                                                          "Colgate Raiders",
                                                          "Colorado Buffaloes",
                                                          "Colorado College Tigers",
                                                          "Colorado State Rams",
                                                          "Columbia Lions",
                                                          "Connecticut Huskies",
                                                          "Coppin State Eagles",
                                                          "Cornell Big Red",
                                                          "Creighton Bluejays",
                                                          "Dallas Baptist Patriots",
                                                          "Dartmouth Big Green",
                                                          "Davidson Wildcats",
                                                          "Dayton Flyers",
                                                          "Delaware Fightin' Blue Hens",
                                                          "Delaware State Hornets",
                                                          "Denver Pioneers",
                                                          "DePaul Blue Demons",
                                                          "Detroit Titans",
                                                          "Drake Bulldogs",
                                                          "Drexel Dragons",
                                                          "Duke Blue Devils",
                                                          "Duquesne Dukes",
                                                          "East Carolina Pirates",
                                                          "East Tennessee State Buccaneers",
                                                          "Eastern Illinois Panthers",
                                                          "Eastern Kentucky Colonels",
                                                          "Eastern Michigan Eagles",
                                                          "Eastern Washington Eagles",
                                                          "Elon Phoenix",
                                                          "Evansville Purple Aces",
                                                          "Fairfield Stags",
                                                          "Fairleigh Dickinson Devils",
                                                          "Fairleigh Dickinson Knights",
                                                          "FIU Panthers",
                                                          "Florida A&M Rattlers",
                                                          "Florida Atlantic Owls",
                                                          "Florida Gators",
                                                          "Florida Gulf Coast Eagles",
                                                          "Florida International Golden Panthers",
                                                          "Florida State Seminoles",
                                                          "Fordham Rams",
                                                          "Fort Wayne Mastodons",
                                                          "Fresno State Bulldogs",
                                                          "Furman Paladins",
                                                          "Gardner-Webb Runnin' Bulldogs",
                                                          "George Mason Patriots",
                                                          "George Washington Colonials",
                                                          "Georgetown Hoyas",
                                                          "Georgia Bulldogs",
                                                          "Georgia Southern Eagles",
                                                          "Georgia State Panthers",
                                                          "Georgia Tech Yellow Jackets",
                                                          "Gonzaga Bulldogs",
                                                          "Grambling Tigers",
                                                          "Grand Canyon Antelopes",
                                                          "Hampton Pirates",
                                                          "Hartford Hawks",
                                                          "Harvard Crimson",
                                                          "Hawaii Rainbow Warriors",
                                                          "High Point Panthers",
                                                          "Hofstra Flying Dutchmen",
                                                          "Hofstra Pride",
                                                          "Holy Cross Crusaders",
                                                          "Houston Baptist Huskies",
                                                          "Houston Cougars",
                                                          "Howard Bison",
                                                          "Idaho State Bengals",
                                                          "Idaho Vandals",
                                                          "Illinois Chicago Flames",
                                                          "Illinois Illini",
                                                          "Illinois State Redbirds",
                                                          "Incarnate Word Cardinals",
                                                          "Indiana Hoosiers",
                                                          "Indiana State Sycamores",
                                                          "Iona Gaels",
                                                          "Iowa Hawkeyes",
                                                          "Iowa State Cyclones",
                                                          "IPFW Mastodons",
                                                          "IUPUI Jaguars",
                                                          "Jackson State Tigers",
                                                          "Jacksonville Dolphins",
                                                          "Jacksonville State Gamecocks",
                                                          "James Madison Dukes",
                                                          "Kansas Jayhawks",
                                                          "Kansas State Wildcats",
                                                          "Kennesaw State Owls",
                                                          "Kent State Golden Flashes",
                                                          "Kentucky Wildcats",
                                                          "La Salle Explorers",
                                                          "Lafayette Leopards",
                                                          "Lamar Cardinals",
                                                          "Lehigh Mountain Hawks",
                                                          "Liberty Flames",
                                                          "Lipscomb Bisons",
                                                          "Long Beach State 49ers",
                                                          "Long Beach State Sharks",
                                                          "Long Island Blackbirds",
                                                          "Longwood Lancers",
                                                          "Louisiana Lafayette Ragin' Cajuns",
                                                          "Louisiana Monroe Indians",
                                                          "Louisiana Tech Bulldogs",
                                                          "Louisiana-Monroe Warhawks",
                                                          "Louisville Cardinals",
                                                          "Loyola Chicago Ramblers",
                                                          "Loyola Maryland Greyhounds",
                                                          "Loyola Marymount Lions",
                                                          "LSU Tigers",
                                                          "Maine Black Bears",
                                                          "Manhattan Jaspers",
                                                          "Marist Red Foxes",
                                                          "Marquette Golden Eagles",
                                                          "Marshall Thundering Herd",
                                                          "Maryland Baltimore County Retrievers",
                                                          "Maryland Eastern Shore Fighting Hawks",
                                                          "Maryland Terrapins",
                                                          "Massachusetts Minutemen",
                                                          "McNeese State Cowboys",
                                                          "Memphis Tigers",
                                                          "Mercer Bears",
                                                          "Miami (Ohio) Redhawks",
                                                          "Miami Hurricanes",
                                                          "Michigan State Spartans",
                                                          "Michigan Wolverines",
                                                          "Middle Tennessee State Blue Raiders",
                                                          "Minnesota Golden Gophers",
                                                          "Mississippi Old Miss Rebels",
                                                          "Mississippi State Bulldogs",
                                                          "Mississippi Valley State Delta Devils",
                                                          "Missouri Kansas City Kangaroos",
                                                          "Missouri Tigers",
                                                          "Monmouth Hawks",
                                                          "Montana Grizzlies",
                                                          "Montana State Bobcats",
                                                          "Morehead State Eagles",
                                                          "Morgan State Bears",
                                                          "Mount St. Mary's Mountaineers",
                                                          "Murray State Racers",
                                                          "Navy Midshipmen",
                                                          "Nebraska Cornhuskers",
                                                          "Nevada Wolf Pack",
                                                          "New Hampshire Wildcats",
                                                          "New Mexico Lobos",
                                                          "New Mexico State Aggies",
                                                          "New Orleans Privateers",
                                                          "Niagara Purple Eagles",
                                                          "Nicholls State Colonels",
                                                          "NJIT Highlanders",
                                                          "Norfolk State Spartans",
                                                          "North Alabama Lions",
                                                          "North Carolina A&T Aggies",
                                                          "North Carolina Asheville Bulldogs",
                                                          "North Carolina Central Eagles",
                                                          "North Carolina Charlotte 49ers",
                                                          "North Carolina Greensboro Spartans",
                                                          "North Carolina State Wolfpack",
                                                          "North Carolina Tar Heels",
                                                          "North Carolina Wilmington Seahawks",
                                                          "North Dakota",
                                                          "North Dakota Fighting Hawks",
                                                          "North Dakota Fighting Sioux",
                                                          "North Dakota State Bison",
                                                          "North Florida Ospreys",
                                                          "North Texas Mean Green",
                                                          "Northeastern Huskies",
                                                          "Northeastern Illinois Golden Eagles",
                                                          "Northern Arizona Lumberjacks",
                                                          "Northern Colorado Bears",
                                                          "Northern Illinois Huskies",
                                                          "Northern Iowa Panthers",
                                                          "Northern Kentucky Norse",
                                                          "Northwestern State Demons",
                                                          "Northwestern Wildcats",
                                                          "Notre Dame Fighting Irish",
                                                          "NYIT Bears",
                                                          "NYU Bobcats",
                                                          "NYU Violets",
                                                          "Oakland Golden Grizzlies",
                                                          "Ohio Bobcats",
                                                          "Ohio State Buckeyes",
                                                          "Oklahoma Sooners",
                                                          "Oklahoma State Cowboys",
                                                          "Old Dominion Monarchs",
                                                          "Ole Miss Rebels",
                                                          "Omaha Mavericks",
                                                          "Oral Roberts Golden Eagles",
                                                          "Oregon Ducks",
                                                          "Oregon State Beavers",
                                                          "Pacific Boxers",
                                                          "Pacific Tigers",
                                                          "Penn Quakers",
                                                          "Penn State Nittany Lions",
                                                          "Pennsylvania Quakers",
                                                          "Pepperdine Waves",
                                                          "Pittsburgh Panthers",
                                                          "Portland Pilots",
                                                          "Portland State Vikings",
                                                          "Prairie View Panthers",
                                                          "Presbyterian Blue Hose",
                                                          "Princeton Tigers",
                                                          "Providence Friars",
                                                          "Purdue Boilermakers",
                                                          "Quinnipiac Bobcats",
                                                          "Radford Highlanders",
                                                          "Rhode Island Rams",
                                                          "Rice Owls",
                                                          "Richmond Spiders",
                                                          "Rider Broncs",
                                                          "Robert Morris Colonials",
                                                          "Rutgers Scarlet Knights",
                                                          "Sacred Heart Pioneers",
                                                          "Saint Mary's Gaels",
                                                          "Sam Houston State Bearkats",
                                                          "Samford Bulldogs",
                                                          "San Diego State Aztecs",
                                                          "San Diego Toreros",
                                                          "San Francisco Dons",
                                                          "San Jose State Spartans",
                                                          "Santa Clara Broncos",
                                                          "Savannah State Tigers",
                                                          "Seattle Redhawks",
                                                          "Seton Hall Pirates",
                                                          "Siena Saints",
                                                          "SIU Edwardsville Cougars",
                                                          "SMU Mustangs",
                                                          "South Alabama Jaguars",
                                                          "South Carolina Fighting Gamecocks",
                                                          "South Carolina State Bulldogs",
                                                          "South Dakota Coyotes",
                                                          "South Dakota State Jackrabbits",
                                                          "South Florida Bulls",
                                                          "Southeast Missouri State Indians",
                                                          "Southeast Missouri State Redhawks",
                                                          "Southeastern Louisiana Lions",
                                                          "Southern Illinois Salukis",
                                                          "Southern Jaguars",
                                                          "Southern Mississippi Golden Eagles",
                                                          "Southern Utah Thunderbirds",
                                                          "Southwest Missouri State Bears",
                                                          "St. Bonaventure Bonnies",
                                                          "St. Francis (New York) Terriers",
                                                          "St. Francis (Pennsylvania) Red Flash",
                                                          "St. Francis Brooklyn Terriers",
                                                          "St. John's Red Storm",
                                                          "St. Joseph's Hawks",
                                                          "St. Louis University Billikens",
                                                          "St. Mary's Rattlers",
                                                          "St. Peter's Peacocks",
                                                          "Stanford Cardinal",
                                                          "Stephen F. Austin Lumberjacks",
                                                          "Stetson Hatters",
                                                          "Stony Brook Seawolves",
                                                          "Syracuse Orange",
                                                          "TCU Horned Frogs",
                                                          "Temple Owls",
                                                          "Tennessee Chattanooga Mocs",
                                                          "Tennessee Martin Skyhawks",
                                                          "Tennessee State Tigers",
                                                          "Tennessee Tech Golden Eagles",
                                                          "Tennessee Volunteers",
                                                          "Texas A&M Aggies",
                                                          "Texas A&M-Corpus Christi Islanders",
                                                          "Texas Arlington Mavericks",
                                                          "Texas El Paso Miners",
                                                          "Texas Longhorns",
                                                          "Texas Pan American Broncs",
                                                          "Texas San Antonio Roadrunners",
                                                          "Texas Southern Tigers",
                                                          "Texas State Bobcats",
                                                          "Texas Tech Red Raiders",
                                                          "Texas-Rio Grande Valley Vaqueros",
                                                          "Toledo Rockets",
                                                          "Towson Tigers",
                                                          "Troy State Trojans",
                                                          "Tulane Green Wave",
                                                          "Tulsa Golden Hurricane",
                                                          "UC Davis Aggies",
                                                          "UCLA Bruins",
                                                          "UMass Lowell River Hawks",
                                                          "UNLV Rebels",
                                                          "USC Trojans",
                                                          "USC Upstate Spartans",
                                                          "Utah State Aggies",
                                                          "Utah Utes",
                                                          "Utah Valley Wolverines",
                                                          "Valparaiso Crusaders",
                                                          "Vanderbilt Commodores",
                                                          "Vermont Catamounts",
                                                          "Villanova Wildcats",
                                                          "Virginia Cavaliers",
                                                          "Virginia Commonwealth Rams",
                                                          "Virginia Tech Hokies",
                                                          "VMI Keydets",
                                                          "Wagner Seahawks",
                                                          "Wake Forest Demon Deacons",
                                                          "Washington Huskies",
                                                          "Washington State Cougars",
                                                          "Weber State Wildcats",
                                                          "West Virginia Mountaineers",
                                                          "Western Carolina Catamounts",
                                                          "Western Illinois Leathernecks",
                                                          "Western Kentucky Hilltoppers",
                                                          "Western Michigan Broncos",
                                                          "Wichita State Shockers",
                                                          "William & Mary Tribe",
                                                          "Winthrop Eagles",
                                                          "Wisconsin Badgers",
                                                          "Wisconsin Green Bay Phoenix",
                                                          "Wisconsin Milwaukee Panthers",
                                                          "Wofford Terriers",
                                                          "Wright State Raiders",
                                                          "Wyoming Cowboys",
                                                          "Xavier Musketeers",
                                                          "Yale Bulldogs",
                                                          "Youngstown State Penguins"
                                                        ]
                                                      }
                                                    }
                                                  }
                                                }
                                              }
                                            }
                                          },
                                          "then": {
                                            "properties": {
                                              "team_name": {
                                                "items": {
                                                  "properties": {
                                                    "value": {
                                                      "enum": [
                                                        "Atlanta United FC",
                                                        "Austin FC",
                                                        "C.D. Chivas USA",
                                                        "Chicago Fire",
                                                        "Colorado Rapids",
                                                        "Columbus Crew",
                                                        "D.C. United",
                                                        "FC Cincinnati",
                                                        "FC Dallas",
                                                        "Houston Dynamo",
                                                        "Inter Miami CF",
                                                        "Los Angeles FC",
                                                        "Los Angeles Galaxy",
                                                        "Minnesota United FC",
                                                        "Montreal Impact",
                                                        "Nashville SC",
                                                        "New England Revolution",
                                                        "New York City FC",
                                                        "New York Red Bulls",
                                                        "Orlando City SC",
                                                        "Philadelphia Union",
                                                        "Portland Timbers",
                                                        "Real Salt Lake",
                                                        "San Jose Earthquakes",
                                                        "Seattle Sounders FC",
                                                        "Sporting Kansas City",
                                                        "St. Louis City",
                                                        "Toronto FC",
                                                        "Vancouver Whitecaps"
                                                      ]
                                                    }
                                                  }
                                                }
                                              }
                                            }
                                          }
                                        },
                                        "then": {
                                          "properties": {
                                            "team_name": {
                                              "items": {
                                                "properties": {
                                                  "value": {
                                                    "enum": [
                                                      "Belenenses",
                                                      "Benfica",
                                                      "Boavista",
                                                      "Casa Pia AC",
                                                      "CD Santa Clara",
                                                      "CF Estrela",
                                                      "Chaves",
                                                      "Desportivo das Aves",
                                                      "Estoril",
                                                      "Famalicão",
                                                      "Farense",
                                                      "FC Arouca",
                                                      "Gil Vicente",
                                                      "Marítimo",
                                                      "Moreirense",
                                                      "Paços de Ferreira",
                                                      "Portimonense SC",
                                                      "Porto",
                                                      "Rio Ave",
                                                      "Sporting",
                                                      "Sporting de Braga",
                                                      "Tondela",
                                                      "Vitória Guimarães",
                                                      "Vitória Setúbal"
                                                    ]
                                                  }
                                                }
                                              }
                                            }
                                          }
                                        }
                                      },
                                      "then": {
                                        "properties": {
                                          "team_name": {
                                            "items": {
                                              "properties": {
                                                "value": {
                                                  "enum": [
                                                    "Arsenal de Sarandí",
                                                    "AS Roma",
                                                    "Boca Juniors",
                                                    "CA River Plate",
                                                    "Club Atlético River Plate",
                                                    "FC Arsenal Tula",
                                                    "FC Basel",
                                                    "FC Startak Moscow",
                                                    "Galatasaray SK",
                                                    "Sao Paulo FC",
                                                    "Sport Club Corinthians Paulista"
                                                  ]
                                                }
                                              }
                                            }
                                          }
                                        }
                                      }
                                    },
                                    "then": {
                                      "properties": {
                                        "team_name": {
                                          "items": {
                                            "properties": {
                                              "value": {
                                                "enum": [
                                                  "Awadhe Warriors",
                                                  "Bengaluru Raptors",
                                                  "Chennai Superstarz",
                                                  "Hyderabad Hunters",
                                                  "Mumbai Rockets",
                                                  "North Eastern Warriors",
                                                  "Pune 7 Aces"
                                                ]
                                              }
                                            }
                                          }
                                        }
                                      }
                                    }
                                  },
                                  "then": {
                                    "properties": {
                                      "team_name": {
                                        "items": {
                                          "properties": {
                                            "value": {
                                              "enum": [
                                                "ALBA Berlin Basketball",
                                                "Anadolu Efes Istanbul Basketball",
                                                "AX Armani Exchange Milan Basketball",
                                                "Barcelona Basketball",
                                                "Bayern Munich Basketball",
                                                "Crvena Zvezda mts Belgrade Basketball",
                                                "CSKA Moscow Basketball",
                                                "Fenerbahce Beko Istanbul",
                                                "Khimki Moscow Region Basketball",
                                                "KIROLBET Baskonia Vitoria-Gasteiz Basketball",
                                                "LDLC ASVEL Villeurbanne",
                                                "Maccabi FOX Tel Aviv Basketball",
                                                "Olympiacos Basketball",
                                                "Panathinaikos Basketball",
                                                "Real Madrid Basketball",
                                                "Valencia Basketball",
                                                "Zalgiris Kaunas Basketball",
                                                "Zenit St Petersburg Basketball"
                                              ]
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                },
                                "then": {
                                  "properties": {
                                    "team_name": {
                                      "items": {
                                        "properties": {
                                          "value": {
                                            "enum": [
                                              "Anaheim Ducks",
                                              "Arizona Coyotes",
                                              "Atlanta Flames",
                                              "Atlanta Thrashers",
                                              "Boston Bruins",
                                              "Buffalo Sabres",
                                              "Calgary Flames",
                                              "California Seals",
                                              "Carolina Hurricanes",
                                              "Chicago Blackhawks",
                                              "Cleveland Barons",
                                              "Colorado Avalanche",
                                              "Columbus Blue Jackets",
                                              "Dallas Stars",
                                              "Detroit Cougars",
                                              "Detroit Falcons",
                                              "Detroit Red Wings",
                                              "Edmonton Oilers",
                                              "Florida Panthers",
                                              "Hamilton Tigers",
                                              "Hartford Whalers",
                                              "Kansas City Scouts",
                                              "Los Angeles Kings",
                                              "Minnesota North Stars",
                                              "Minnesota Wild",
                                              "Montreal Canadiens",
                                              "Montreal Maroons",
                                              "Montreal Wanderers",
                                              "Nashville Predators",
                                              "New Jersey Devils",
                                              "New York Americans",
                                              "New York Islanders",
                                              "New York Rangers",
                                              "Ottawa Senators",
                                              "Philadelphia Flyers",
                                              "Philadelphia Quakers",
                                              "Pittsburgh Penguins",
                                              "San Jose Sharks",
                                              "Seattle Kraken",
                                              "St. Louis Blues",
                                              "St. Louis Eagles",
                                              "Tampa Bay Lightning",
                                              "Toronto Arenas",
                                              "Toronto Maple Leafs",
                                              "Toronto St. Pats",
                                              "Utah Mammoth",
                                              "Vancouver Canucks",
                                              "Vegas Golden Knights",
                                              "Washington Capitals",
                                              "Winnipeg Jets"
                                            ]
                                          }
                                        }
                                      }
                                    }
                                  }
                                }
                              },
                              "then": {
                                "properties": {
                                  "team_name": {
                                    "items": {
                                      "properties": {
                                        "value": {
                                          "enum": [
                                            "Aberdeen IronBirds",
                                            "Akron Aeros",
                                            "Albuquerque Isotopes",
                                            "Altoona Curve",
                                            "Arkansas Travelers",
                                            "Asheville Tourists",
                                            "Auburn Doubledays",
                                            "Augusta GreenJackets",
                                            "Bakersfield Blaze",
                                            "Batavia Muckdogs",
                                            "Beloit Snappers",
                                            "Billings Mustangs",
                                            "Binghamton Mets",
                                            "Birmingham Barons",
                                            "Bluefield Orioles",
                                            "Boise Hawks",
                                            "Bowie Baysox",
                                            "Bowling Green Hot Rods",
                                            "Bradenton Marauders",
                                            "Brevard County Manatees",
                                            "Bristol White Sox",
                                            "Brooklyn Cyclones",
                                            "Buffalo Bisons",
                                            "Burlington Bees",
                                            "Burlington Royals",
                                            "Carolina Mudcats",
                                            "Casper Ghosts",
                                            "Cedar Rapids Kernels",
                                            "Charleston RiverDogs",
                                            "Charlotte Knights",
                                            "Charlotte Stone Crabs",
                                            "Chattanooga Lookouts",
                                            "Clearwater Threshers",
                                            "Clinton LumberKings",
                                            "Colorado Springs Sky Sox",
                                            "Columbus Clippers",
                                            "Connecticut Tigers",
                                            "Corpus Christi Hooks",
                                            "Danville Braves",
                                            "Dayton Dragons",
                                            "Daytona Cubs",
                                            "Delmarva Shorebirds",
                                            "Dunedin Blue Jays",
                                            "Durham Bulls",
                                            "Elizabethton Twins",
                                            "Erie SeaWolves",
                                            "Eugene Emeralds",
                                            "Everett AquaSox",
                                            "Fort Myers Miracle",
                                            "Fort Wayne TinCaps",
                                            "Frederick Keys",
                                            "Fresno Grizzlies",
                                            "Frisco RoughRiders",
                                            "Great Falls Voyagers",
                                            "Great Lakes Loons",
                                            "Greeneville Astros",
                                            "Greensboro Grasshoppers",
                                            "Greenville Drive",
                                            "Gwinnett Braves",
                                            "Hagerstown Suns",
                                            "Harrisburg Senators",
                                            "Helena Brewers",
                                            "Hickory Crawdads",
                                            "High Desert Mavericks",
                                            "Hudson Valley Renegades",
                                            "Huntsville Stars",
                                            "Idaho Falls Chukars",
                                            "Indianapolis Indians",
                                            "Inland Empire 66ers",
                                            "Iowa Cubs",
                                            "Jacksonville Suns",
                                            "Jamestown Jammers",
                                            "Johnson City Cardinals",
                                            "Jupiter Hammerheads",
                                            "Kane County Cougars",
                                            "Kannapolis Intimidators",
                                            "Kingsport Mets",
                                            "Kinston Indians",
                                            "Lake County Captains",
                                            "Lake Elsinore Storm",
                                            "Lakeland Flying Tigers",
                                            "Lakewood BlueClaws",
                                            "Lancaster JetHawks",
                                            "Lansing Lugnuts",
                                            "Las Vegas 51s",
                                            "Lehigh Valley IronPigs",
                                            "Lexington Legends",
                                            "Louisville Bats",
                                            "Lowell Spinners",
                                            "Lynchburg Hillcats",
                                            "Mahoning Valley Scrappers",
                                            "Memphis Redbirds",
                                            "Midland RockHounds",
                                            "Mississippi Braves",
                                            "Missoula Osprey",
                                            "Mobile BayBears",
                                            "Modesto Nuts",
                                            "Montgomery Biscuits",
                                            "Myrtle Beach Pelicans",
                                            "Nashville Sounds",
                                            "New Britain Rock Cats",
                                            "New Hampshire Fisher Cats",
                                            "New Orleans Zephyrs",
                                            "Norfolk Tides",
                                            "Northwest Arkansas Naturals",
                                            "Ogden Raptors",
                                            "Oklahoma City RedHawks",
                                            "Omaha Royals",
                                            "Orem Owlz",
                                            "Palm Beach Cardinals",
                                            "Pawtucket Red Sox",
                                            "Peoria Chiefs",
                                            "Portland Beavers",
                                            "Portland Sea Dogs",
                                            "Potomac Nationals",
                                            "Princeton Rays",
                                            "Pulaski Mariners",
                                            "Quad Cities River Bandits",
                                            "Rancho Cucamonga Quakes",
                                            "Reading Phillies",
                                            "Reno Aces",
                                            "Richmond Flying Squirrels",
                                            "Rochester Red Wings",
                                            "Rome Braves",
                                            "Round Rock Express",
                                            "Sacramento River Cats",
                                            "Salem Red Sox",
                                            "Salem-Keizer Volcanoes",
                                            "Salt Lake Bees",
                                            "San Antonio Missions",
                                            "San Jose Giants",
                                            "Savannah Sand Gnats",
                                            "Scranton/Wilkes-Barre Yankees",
                                            "South Bend Silver Hawks",
                                            "Spokane Indians",
                                            "Springfield Cardinals",
                                            "St. Lucie Mets",
                                            "State College Spikes",
                                            "Staten Island Yankees",
                                            "Stockton Ports",
                                            "Syracuse Chiefs",
                                            "Tacoma Rainiers",
                                            "Tampa Yankees",
                                            "Tennessee Smokies",
                                            "Toledo Mud Hens",
                                            "Trenton Thunder",
                                            "Tri-City Dust Devils",
                                            "Tri-City ValleyCats",
                                            "Tulsa Drillers",
                                            "Vancouver Canadians",
                                            "Vermont Lake Monsters",
                                            "Visalia Rawhide",
                                            "Washington Nationals",
                                            "West Michigan Whitecaps",
                                            "West Tenn Diamond Jaxx",
                                            "West Virginia Power",
                                            "Williamsport Crosscutters",
                                            "Wilmington Blue Rocks",
                                            "Winston-Salem Dash",
                                            "Wisconsin Timber Rattlers",
                                            "Yakima Bears"
                                          ]
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            },
                            "then": {
                              "properties": {
                                "team_name": {
                                  "items": {
                                    "properties": {
                                      "value": {
                                        "enum": [
                                          "Atlanta Hawks",
                                          "Boston Celtics",
                                          "Brooklyn Nets",
                                          "Buffalo Braves",
                                          "Charlotte Hornets",
                                          "Chicago Bulls",
                                          "Chicago Stags",
                                          "Chicago Zephyrs",
                                          "Cleveland Cavaliers",
                                          "Dallas Mavericks",
                                          "Denver Nuggets",
                                          "Detroit Pistons",
                                          "Fort Wayne Pistons",
                                          "Golden State Warriors",
                                          "Houston Rockets",
                                          "Indiana Pacers",
                                          "Kansas City Kings",
                                          "Los Angeles Clippers",
                                          "Los Angeles Lakers",
                                          "Memphis Grizzlies",
                                          "Miami Heat",
                                          "Milwaukee Bucks",
                                          "Milwaukee Hawks",
                                          "Minnesota Timberwolves",
                                          "New Jersey Nets",
                                          "New Orleans Pelicans",
                                          "New York Knicks",
                                          "Oklahoma City Thunder",
                                          "Orlando Magic",
                                          "Philadelphia 76ers",
                                          "Phoenix Suns",
                                          "Portland Trail Blazers",
                                          "Rochester Royals",
                                          "Sacramento Kings",
                                          "San Antonio Spurs",
                                          "San Diego Clippers",
                                          "San Diego Rockets",
                                          "San Francisco Warriors",
                                          "Seattle SuperSonics",
                                          "St. Louis Bombers",
                                          "St. Louis Hawks",
                                          "Syracuse Nationals",
                                          "Toronto Raptors",
                                          "Utah Jazz",
                                          "Washington Wizards"
                                        ]
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          },
                          "then": {
                            "properties": {
                              "team_name": {
                                "items": {
                                  "properties": {
                                    "value": {
                                      "enum": [
                                        "BC Lions",
                                        "Calgary Stampeders",
                                        "Edmonton Football Team",
                                        "Hamilton Tiger-Cats",
                                        "Montreal Alouettes",
                                        "Ottawa Redblacks",
                                        "Saskatchewan Roughriders",
                                        "Toronto Argonauts",
                                        "Winnipeg Blue Bombers"
                                      ]
                                    }
                                  }
                                }
                              }
                            }
                          }
                        },
                        "then": {
                          "properties": {
                            "team_name": {
                              "items": {
                                "properties": {
                                  "value": {
                                    "enum": [
                                      "AD Alcorcón",
                                      "Alaves",
                                      "Albacete BP",
                                      "Athletic Bilbao",
                                      "Atletico Madrid",
                                      "Barcelona",
                                      "Betis Sevilla",
                                      "CD Lugo",
                                      "CD Mirandés",
                                      "CD Numancia",
                                      "CD Tenerife",
                                      "Celta Vigo",
                                      "CF Fuenlabrada",
                                      "Cádiz CF",
                                      "Deportivo La Coruna",
                                      "Elche CF",
                                      "Espanyol",
                                      "Extremadura UD",
                                      "FC Sevilla",
                                      "Getafe CF",
                                      "Getafe FC",
                                      "Girona FC",
                                      "Granada CF",
                                      "Leganés",
                                      "Levante UD",
                                      "Malaga",
                                      "Mallorca",
                                      "Osasuna",
                                      "Racing Santander",
                                      "Rayo Vallecano",
                                      "Real Madrid",
                                      "Real Oviedo",
                                      "Real Sociedad",
                                      "Real Zaragoza",
                                      "Recreativo Huelva",
                                      "SD Eibar",
                                      "SD Huesca",
                                      "SD Ponferradina",
                                      "Sporting Gijón",
                                      "UD Almería",
                                      "UD Las Palmas",
                                      "Valencia",
                                      "Valladolid",
                                      "Villareal"
                                    ]
                                  }
                                }
                              }
                            }
                          }
                        }
                      },
                      "then": {
                        "properties": {
                          "team_name": {
                            "items": {
                              "properties": {
                                "value": {
                                  "enum": [
                                    "Atlético Ottawa",
                                    "Cavalry FC",
                                    "FC Edmonton",
                                    "Forge FC",
                                    "HFX Wanderers FC",
                                    "Pacific FC",
                                    "Valour FC",
                                    "Vancouver FC",
                                    "York United FC"
                                  ]
                                }
                              }
                            }
                          }
                        }
                      }
                    },
                    "then": {
                      "properties": {
                        "team_name": {
                          "items": {
                            "properties": {
                              "value": {
                                "enum": [
                                  "WUSA"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  },
                  "then": {
                    "properties": {
                      "team_name": {
                        "items": {
                          "properties": {
                            "value": {
                              "enum": [
                                "AFC Bournemouth",
                                "Arsenal",
                                "Aston Villa",
                                "Birmingham City",
                                "Blackburn Rovers",
                                "Bolton Wanderers",
                                "Brentford",
                                "Brighton & Hove Albion",
                                "Bristol City",
                                "Burnley",
                                "Cardiff City",
                                "Charlton Athletic",
                                "Chelsea",
                                "Coventry City",
                                "Crystal Palace",
                                "Derby County",
                                "Everton",
                                "Fulham",
                                "Huddersfield Town",
                                "Hull City",
                                "Ipswich Town",
                                "Leeds United",
                                "Leicester City",
                                "Liverpool",
                                "Luton Town",
                                "Manchester City",
                                "Manchester United",
                                "Middlesbrough",
                                "Millwall",
                                "Newcastle United",
                                "Norwich City",
                                "Nottingham Forest",
                                "Plymouth Argyle",
                                "Preston North End",
                                "QPR",
                                "Reading",
                                "Rotherham United",
                                "Sheffield United",
                                "Sheffield Wednesday",
                                "Southampton",
                                "Stoke City",
                                "Sunderland",
                                "Swansea City",
                                "Tottenham Hotspur",
                                "Watford",
                                "West Bromwich Albion",
                                "West Ham United",
                                "Wigan",
                                "Wolverhampton Wanderers"
                              ]
                            }
                          }
                        }
                      }
                    }
                  }
                },
                "then": {
                  "properties": {
                    "team_name": {
                      "items": {
                        "properties": {
                          "value": {
                            "enum": [
                              "Chiba Lotte Marines",
                              "Chunichi Dragons",
                              "Fukuoka SoftBank Hawks",
                              "Hanshin Tigers",
                              "High School Baseball Team",
                              "Hiroshima Toyo Carp",
                              "Hokkaido Nippon-Ham Fighters",
                              "Orix Buffaloes",
                              "Saitama Seibu Lions",
                              "Tohoku Rakuten Golden Eagles",
                              "Tokyo Yakult Swallows",
                              "Yokohama DeNA BayStars",
                              "Yomiuri Giants"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              "then": {
                "properties": {
                  "team_name": {
                    "items": {
                      "properties": {
                        "value": {
                          "enum": [
                            "Aizawl FC",
                            "Chennai City FC",
                            "Churchill Brothers FC Goa",
                            "Gokulam Kerala FC",
                            "Indian Arrows",
                            "Mohun Bagan",
                            "NEROCA FC",
                            "Punjab FC",
                            "Quess East Bengal",
                            "Real Kashmir FC",
                            "Tiddim Road Athletic Union"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            },
            "then": {
              "properties": {
                "team_name": {
                  "items": {
                    "properties": {
                      "value": {
                        "enum": [
                          "Alfa Romeo Racing",
                          "Alpine",
                          "Aston Martin",
                          "BWT Racing Point",
                          "Haas F1 Team",
                          "Mclaren",
                          "Mercedes-AMG Petronas",
                          "Red Bull Racing",
                          "Renault DP World",
                          "Scuderia AlphaTauri",
                          "Scuderia Ferrari",
                          "Williams Racing"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          "then": {
            "properties": {
              "team_name": {
                "items": {
                  "properties": {
                    "value": {
                      "enum": [
                        "Delhi Sultans",
                        "Haryana Hammers",
                        "MP Yodha",
                        "Mumbai Maharathi",
                        "NCR Punjab Royals",
                        "UP Dangal"
                      ]
                    }
                  }
                }
              }
            }
          }
        },
        "then": {
          "properties": {
            "team_name": {
              "items": {
                "properties": {
                  "value": {
                    "enum": [
                      "E-Sports"
                    ]
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "team_name": {
            "items": {
              "properties": {
                "value": {
                  "enum": [
                    "A. J. Allmendinger",
                    "Alex Bowman",
                    "Aric Almirola",
                    "Austin Dillon",
                    "Bobby Labonte",
                    "Brad Keselowski",
                    "Carl Edwards",
                    "Casey Mears",
                    "Chase Elliott",
                    "Chris Buescher",
                    "Clint Bowyer",
                    "Dale Earnhardt",
                    "Dale Earnhardt Jr.",
                    "Daniel Suárez",
                    "Darrell Wallace Jr.",
                    "David Ragan",
                    "Denny Hamlin",
                    "Elliott Sadler",
                    "Erik Jones",
                    "Gray Gaulding",
                    "Greg Biffle",
                    "Jamie McMurray",
                    "Jeff Burton",
                    "Jeff Gordon",
                    "Jimmie Johnson",
                    "Joey Logano",
                    "Juan Pablo Montoya",
                    "Kasey Kahne",
                    "Kevin Harvick",
                    "Kurt Busch",
                    "Kyle Busch",
                    "Kyle Larson",
                    "Mark Martin",
                    "Martin Truex Jr.",
                    "Matt DiBenedetto",
                    "Matt Kenseth",
                    "Michael McDowell",
                    "Paul Menard",
                    "Richard Petty",
                    "Ricky Stenhouse Jr.",
                    "Ryan Blaney",
                    "Ryan Newman",
                    "Tony Stewart",
                    "Trevor Bayne",
                    "Ty Dillon",
                    "William Byron"
                  ]
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "MODEL_NAME/TEAM_NAME",
                        "TEAM_NAME",
                        "TEAM_NAME/SIZE_NAME"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "team_name"
        ]
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "master_pack_weight"
                ],
                "properties": {
                  "master_pack_weight": {
                    "items": {
                      "required": [
                        "value"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_weight"
                ],
                "properties": {
                  "master_pack_weight": {
                    "items": {
                      "required": [
                        "value"
                      ]
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "master_pack_dimensions"
        ]
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "length"
                      ],
                      "properties": {
                        "length": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "length"
                      ],
                      "properties": {
                        "length": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "width"
                      ],
                      "properties": {
                        "width": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "width"
                      ],
                      "properties": {
                        "width": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "height"
                      ],
                      "properties": {
                        "height": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "master_pack_dimensions"
                ],
                "properties": {
                  "master_pack_dimensions": {
                    "items": {
                      "required": [
                        "height"
                      ],
                      "properties": {
                        "height": {
                          "items": {
                            "required": [
                              "value"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "master_pack_weight"
        ]
      }
    },
    {
      "if": {
        "not": {
          "required": [
            "parentage_level"
          ],
          "properties": {
            "parentage_level": {
              "contains": {
                "required": [
                  "value"
                ],
                "properties": {
                  "value": {
                    "enum": [
                      "child"
                    ]
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "child_parent_sku_relationship": {
            "items": {
              "not": {
                "required": [
                  "parent_sku"
                ]
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "parentage_level"
        ],
        "properties": {
          "parentage_level": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "child"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "child_parent_sku_relationship": {
            "items": {
              "required": [
                "parent_sku"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "parentage_level"
        ],
        "properties": {
          "parentage_level": {
            "items": {
              "required": [
                "value"
              ]
            }
          }
        }
      },
      "then": {
        "required": [
          "child_parent_sku_relationship"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "contains": {
                  "required": [
                    "child_relationship_type"
                  ],
                  "properties": {
                    "child_relationship_type": {
                      "enum": [
                        "variation"
                      ]
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "parentage_level"
            ],
            "properties": {
              "parentage_level": {
                "items": {
                  "required": [
                    "value"
                  ]
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "variation_theme"
        ]
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "required": [
              "fulfillment_availability"
            ],
            "properties": {
              "fulfillment_availability": {
                "contains": {
                  "required": [
                    "fulfillment_channel_code"
                  ],
                  "properties": {
                    "fulfillment_channel_code": {
                      "enum": [
                        "AMAZON_NA"
                      ]
                    }
                  }
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "fulfillment_availability"
              ],
              "properties": {
                "fulfillment_availability": {
                  "items": {
                    "required": [
                      "fulfillment_channel_code"
                    ]
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "batteries_required"
        ]
      }
    },
    {
      "if": {
        "required": [
          "batteries_required"
        ],
        "properties": {
          "batteries_required": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    true
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "batteries_included"
        ]
      }
    },
    {
      "if": {
        "required": [
          "batteries_included"
        ],
        "properties": {
          "batteries_included": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    true
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "battery"
        ],
        "properties": {
          "battery": {
            "items": {
              "required": [
                "cell_composition"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "not": {
          "required": [
            "battery"
          ],
          "properties": {
            "battery": {
              "contains": {
                "required": [
                  "cell_composition"
                ],
                "properties": {
                  "cell_composition": {
                    "contains": {
                      "required": [
                        "value"
                      ],
                      "properties": {
                        "value": {
                          "enum": [
                            "other_than_listed"
                          ]
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "battery": {
            "items": {
              "properties": {
                "cell_composition_other_than_listed": {
                  "not": {
                    "required": [
                      "value"
                    ]
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "battery"
                ],
                "properties": {
                  "battery": {
                    "contains": {
                      "required": [
                        "cell_composition"
                      ],
                      "properties": {
                        "cell_composition": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "other_than_listed"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "battery"
                ],
                "properties": {
                  "battery": {
                    "contains": {
                      "required": [
                        "cell_composition"
                      ],
                      "properties": {
                        "cell_composition": {
                          "contains": {
                            "required": [
                              "value"
                            ],
                            "properties": {
                              "value": {
                                "enum": [
                                  "other_than_listed"
                                ]
                              }
                            }
                          }
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "battery"
        ],
        "properties": {
          "battery": {
            "items": {
              "required": [
                "cell_composition_other_than_listed"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "battery"
        ],
        "properties": {
          "battery": {
            "contains": {
              "required": [
                "cell_composition"
              ],
              "properties": {
                "cell_composition": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "lithium_ion",
                          "lithium_metal",
                          "lithium_polymer"
                        ]
                      }
                    }
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "battery",
          "lithium_battery",
          "num_batteries"
        ],
        "properties": {
          "battery": {
            "items": {
              "required": [
                "weight"
              ]
            }
          },
          "lithium_battery": {
            "items": {
              "required": [
                "packaging"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "battery"
        ],
        "properties": {
          "battery": {
            "contains": {
              "required": [
                "cell_composition"
              ],
              "properties": {
                "cell_composition": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "lithium_metal"
                        ]
                      }
                    }
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "lithium_battery",
          "number_of_lithium_metal_cells"
        ],
        "properties": {
          "lithium_battery": {
            "items": {
              "required": [
                "weight"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "battery"
        ],
        "properties": {
          "battery": {
            "contains": {
              "required": [
                "cell_composition"
              ],
              "properties": {
                "cell_composition": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "lithium_ion",
                          "lithium_polymer"
                        ]
                      }
                    }
                  }
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "lithium_battery",
          "number_of_lithium_ion_cells"
        ],
        "properties": {
          "lithium_battery": {
            "items": {
              "required": [
                "energy_content"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "supplier_declared_dg_hz_regulation"
        ],
        "properties": {
          "supplier_declared_dg_hz_regulation": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "not_applicable"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "supplier_declared_dg_hz_regulation": {
            "items": {
              "properties": {
                "value": {
                  "not": {
                    "enum": [
                      "other",
                      "storage",
                      "transportation",
                      "waste"
                    ]
                  }
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "supplier_declared_dg_hz_regulation"
        ],
        "properties": {
          "supplier_declared_dg_hz_regulation": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "ghs"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "ghs",
          "safety_data_sheet_url"
        ],
        "properties": {
          "ghs": {
            "items": {
              "required": [
                "classification"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "supplier_declared_dg_hz_regulation"
        ],
        "properties": {
          "supplier_declared_dg_hz_regulation": {
            "contains": {
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "transportation"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "required": [
          "hazmat"
        ],
        "properties": {
          "hazmat": {
            "contains": {
              "required": [
                "aspect"
              ],
              "properties": {
                "aspect": {
                  "enum": [
                    "united_nations_regulatory_id"
                  ]
                }
              }
            }
          }
        }
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "ITEM_WEIGHT"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "item_weight"
        ]
      }
    },
    {
      "properties": {
        "california_proposition_65": {
          "items": {
            "if": {
              "required": [
                "compliance_type"
              ],
              "properties": {
                "compliance_type": {
                  "enum": [
                    "food",
                    "furniture",
                    "chemical"
                  ]
                }
              }
            },
            "then": {
              "required": [
                "chemical_names"
              ],
              "properties": {
                "chemical_names": {
                  "minItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "california_proposition_65": {
          "items": {
            "if": {
              "required": [
                "compliance_type"
              ],
              "properties": {
                "compliance_type": {
                  "enum": [
                    "food",
                    "furniture",
                    "chemical"
                  ]
                }
              }
            },
            "else": {
              "not": {
                "required": [
                  "chemical_names"
                ]
              }
            },
            "then": {
              "properties": {
                "chemical_names": {
                  "maxItems": 1
                }
              }
            }
          }
        }
      }
    },
    {
      "properties": {
        "pesticide_marking": {
          "items": {
            "if": {
              "required": [
                "marking_type"
              ],
              "properties": {
                "marking_type": {
                  "enum": [
                    "epa_establishment_number",
                    "epa_registration_number"
                  ]
                }
              }
            },
            "then": {
              "required": [
                "registration_status"
              ]
            }
          }
        }
      }
    },
    {
      "properties": {
        "pesticide_marking": {
          "items": {
            "if": {
              "required": [
                "registration_status"
              ],
              "properties": {
                "registration_status": {
                  "enum": [
                    "fifra_registration_required"
                  ]
                }
              }
            },
            "then": {
              "required": [
                "certification_number"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "fcc_radio_frequency_emission_compliance"
        ],
        "properties": {
          "fcc_radio_frequency_emission_compliance": {
            "contains": {
              "required": [
                "registration_status"
              ],
              "properties": {
                "registration_status": {
                  "enum": [
                    "has_fcc_id"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "fcc_radio_frequency_emission_compliance": {
            "items": {
              "required": [
                "identification_number"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "required": [
          "fcc_radio_frequency_emission_compliance"
        ],
        "properties": {
          "fcc_radio_frequency_emission_compliance": {
            "contains": {
              "required": [
                "registration_status"
              ],
              "properties": {
                "registration_status": {
                  "enum": [
                    "fcc_supplier_declaration_of_conformity"
                  ]
                }
              }
            }
          }
        }
      },
      "then": {
        "properties": {
          "fcc_radio_frequency_emission_compliance": {
            "items": {
              "required": [
                "point_of_contact_address",
                "point_of_contact_email",
                "point_of_contact_name",
                "point_of_contact_phone_number"
              ]
            }
          }
        }
      }
    },
    {
      "if": {
        "anyOf": [
          {
            "allOf": [
              {
                "required": [
                  "fulfillment_availability"
                ],
                "properties": {
                  "fulfillment_availability": {
                    "contains": {
                      "required": [
                        "fulfillment_channel_code"
                      ],
                      "properties": {
                        "fulfillment_channel_code": {
                          "enum": [
                            "AMAZON_NA"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "required": [
                  "fulfillment_availability"
                ],
                "properties": {
                  "fulfillment_availability": {
                    "contains": {
                      "required": [
                        "fulfillment_channel_code"
                      ],
                      "properties": {
                        "fulfillment_channel_code": {
                          "enum": [
                            "AMAZON_NA"
                          ]
                        }
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "fulfillment_availability"
                  ],
                  "properties": {
                    "fulfillment_availability": {
                      "items": {
                        "required": [
                          "fulfillment_channel_code"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "items": {
                        "required": [
                          "value"
                        ]
                      }
                    }
                  }
                }
              }
            ]
          },
          {
            "allOf": [
              {
                "not": {
                  "required": [
                    "fulfillment_availability"
                  ],
                  "properties": {
                    "fulfillment_availability": {
                      "items": {
                        "required": [
                          "fulfillment_channel_code"
                        ]
                      }
                    }
                  }
                }
              },
              {
                "not": {
                  "required": [
                    "parentage_level"
                  ],
                  "properties": {
                    "parentage_level": {
                      "contains": {
                        "required": [
                          "value"
                        ],
                        "properties": {
                          "value": {
                            "enum": [
                              "parent"
                            ]
                          }
                        }
                      }
                    }
                  }
                }
              }
            ]
          }
        ]
      },
      "then": {
        "required": [
          "item_package_dimensions",
          "item_package_weight"
        ]
      }
    },
    {
      "if": {
        "allOf": [
          {
            "required": [
              "child_parent_sku_relationship"
            ],
            "properties": {
              "child_parent_sku_relationship": {
                "items": {
                  "required": [
                    "parent_sku"
                  ]
                }
              }
            }
          },
          {
            "not": {
              "required": [
                "parentage_level"
              ],
              "properties": {
                "parentage_level": {
                  "contains": {
                    "required": [
                      "value"
                    ],
                    "properties": {
                      "value": {
                        "enum": [
                          "parent"
                        ]
                      }
                    }
                  }
                }
              }
            }
          },
          {
            "required": [
              "variation_theme"
            ],
            "properties": {
              "variation_theme": {
                "contains": {
                  "required": [
                    "name"
                  ],
                  "properties": {
                    "name": {
                      "enum": [
                        "ITEM_DISPLAY_WEIGHT/SIZE_NAME",
                        "ITEM_DISPLAY_WEIGHT",
                        "MATERIAL_TYPE/ITEM_DISPLAY_WEIGHT",
                        "COLOR_NAME/ITEM_DISPLAY_WEIGHT",
                        "SIZE_NAME/ITEM_DISPLAY_WEIGHT",
                        "ITEM_DISPLAY_WEIGHT/COLOR_NAME",
                        "ITEM_DISPLAY_WEIGHT/MATERIAL_TYPE"
                      ]
                    }
                  }
                }
              }
            }
          }
        ]
      },
      "then": {
        "required": [
          "item_display_weight"
        ]
      }
    }
  ],
  "$schema": "https://schemas.amazon.com/selling-partners/definitions/product-types/meta-schema/v1",
  "$comment": "Amazon product type definition for MANUAL_FOOD_MILL_GRINDER product type",
  "required": [
    "brand",
    "bullet_point",
    "country_of_origin",
    "item_name",
    "item_type_keyword",
    "product_description",
    "supplier_declared_dg_hz_regulation"
  ],
  "properties": {
    "ghs": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "classification": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "class"
              ],
              "properties": {
                "class": {
                  "enum": [
                    "amzn_specific_no_label_with_warning",
                    "compressed_gas",
                    "corrosive",
                    "environmentally_damaging",
                    "explosive",
                    "flammable",
                    "health_hazard",
                    "irritant",
                    "oxidizing",
                    "toxic"
                  ],
                  "type": "string",
                  "title": "GHS Class",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "Explosive"
                  ],
                  "enumNames": [
                    "Amazon Specific No Label With Warning",
                    "Compressed Gas",
                    "Corrosive",
                    "Environmentally Damaging",
                    "Explosive",
                    "Flammable",
                    "Health Hazard",
                    "Irritant",
                    "Oxidizing",
                    "Toxic"
                  ],
                  "description": "Select the GHS Class of the product from the list of valid values if GHS is selected as the Dangerous Goods Regulation. GHS Class indicates the warning statement assigned by the GHS classification system."
                }
              },
              "additionalProperties": false
            },
            "title": "GHS Classification",
            "examples": [
              "Class: Explosive, Subcategory: Liquid"
            ],
            "minItems": 1,
            "selectors": [
              "class"
            ],
            "description": "Provide the Global Harmonized System (GHS) CLP classification for the product",
            "maxUniqueItems": 1000,
            "minUniqueItems": 1
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "GHS",
      "examples": [
        "NGK"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the Global Harmonized System (GHS) information",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "size": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Size",
            "hidden": false,
            "editable": true,
            "examples": [
              "Extra Large"
            ],
            "maxLength": 50,
            "description": "Provide the size of the item",
            "maxUtf8ByteLength": 2000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Size",
      "examples": [
        "2T, 6X, 12, Small, X-Large, 18 months, 14 Tall, 28Wx32L"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "The numeric or text version of the item's size.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "brand": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Brand Name",
            "hidden": false,
            "editable": false,
            "examples": [
              "Sony"
            ],
            "maxLength": 100,
            "minLength": 1,
            "description": "Provide the brand name of the product"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Brand Name",
      "examples": [
        "Sonny Brook Hams"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Max. 50 characters",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "color": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Color",
            "hidden": false,
            "editable": true,
            "examples": [
              "Cranberry"
            ],
            "maxLength": 1000,
            "minLength": 0,
            "description": "Provide the color of the product"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "standardized_values": {
            "type": "array",
            "items": {
              "type": "string"
            },
            "title": "Color Map",
            "hidden": false,
            "editable": true,
            "examples": [
              "Red"
            ],
            "maxItems": 1,
            "minItems": 1,
            "description": "Select the most dominant color of the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Color",
      "examples": [
        "Cranberry"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide the color of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "style": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Style",
            "hidden": false,
            "editable": true,
            "examples": [
              "Art Deco"
            ],
            "maxLength": 2200,
            "description": "Provide the style of the product. Style refers to the aesthetic choices of a person or a group of people. It describes the distinctive visual representation of a product",
            "maxUtf8ByteLength": 2000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Style Name",
      "examples": [
        "Mission; Art Deco; Jack Purcell"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "The style of the item",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "flavor": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Flavor",
            "hidden": false,
            "editable": true,
            "examples": [
              "Double Rich Chocolate, Cherry, Chocolate, Vanilla"
            ],
            "maxLength": 2200,
            "description": "Specify the flavor of the product"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Flavor",
      "examples": [
        "Double Rich Chocolate, Cherry, Chocolate, Vanilla"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "What flavor is the product?",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "hazmat": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "aspect",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Hazmat",
            "hidden": false,
            "editable": false,
            "examples": [
              "UN1993"
            ],
            "maxLength": 2197,
            "description": "Provide hazmat information that is relevant to the product based on the aspect selected"
          },
          "aspect": {
            "enum": [
              "united_nations_regulatory_id"
            ],
            "type": "string",
            "title": "Hazmat Aspect",
            "hidden": false,
            "editable": false,
            "examples": [
              "UN Regulatory Id"
            ],
            "enumNames": [
              "UN Regulatory Id"
            ],
            "description": "Select the aspect or regulatory body used for the hazardous product information"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Hazmat",
      "examples": [
        "UN1993"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "aspect"
      ],
      "description": "Provide hazmat information that is relevant to the product based on the aspect selected",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "battery": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "weight": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "unit",
                "value"
              ],
              "properties": {
                "unit": {
                  "enum": [
                    "grams",
                    "hundredths_pounds",
                    "kilograms",
                    "milligrams",
                    "ounces",
                    "pounds",
                    "tons"
                  ],
                  "type": "string",
                  "title": "Battery Weight Unit",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "Grams"
                  ],
                  "enumNames": [
                    "Grams",
                    "Hundredths Pounds",
                    "Kilograms",
                    "Milligrams",
                    "Ounces",
                    "Pounds",
                    "Tons"
                  ],
                  "description": "Provide unit for battery weight"
                },
                "value": {
                  "type": "number",
                  "title": "Battery Weight",
                  "hidden": false,
                  "minimum": 0,
                  "editable": true,
                  "examples": [
                    "2.5"
                  ],
                  "maxLength": 5000,
                  "description": "Provide the total net weight (numeric value) of the batteries included. This is the weight of the standalone batteries not including packaging or the device it may be used in."
                }
              },
              "additionalProperties": false
            },
            "title": "Battery Weight",
            "examples": [
              "2.5 Grams"
            ],
            "maxItems": 1,
            "minItems": 1,
            "description": "Provide the total net weight of the batteries included. This is the weight of the standalone batteries not including packaging or the device it may be used in"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "cell_composition": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "alkaline",
                    "lead_acid",
                    "lithium_ion",
                    "lithium_metal",
                    "lithium_polymer",
                    "NiCAD",
                    "NiMh",
                    "other_than_listed",
                    "sodium_ion",
                    "wet_alkali"
                  ],
                  "type": "string",
                  "title": "Battery Cell Composition",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "NiMh"
                  ],
                  "enumNames": [
                    "Alkaline",
                    "Lead Acid",
                    "Lithium Ion",
                    "Lithium Metal",
                    "Lithium Polymer",
                    "NiCAD",
                    "NiMH",
                    "Other Than Listed",
                    "Sodium Ion",
                    "Wet Alkali"
                  ],
                  "description": "Select the chemical composition of the battery cell"
                }
              },
              "additionalProperties": false
            },
            "title": "Battery Type",
            "examples": [
              "NiMh, lithium_ion"
            ],
            "maxItems": 1,
            "minItems": 1,
            "description": "What type or composition is the battery?"
          },
          "cell_composition_other_than_listed": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "language_tag",
                "value"
              ],
              "properties": {
                "value": {
                  "type": "string",
                  "title": "Battery Cell Composition Other Than Listed",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "Silver Oxide (Ag₂O)"
                  ],
                  "maxLength": 50,
                  "description": "Provide the components of the item's battery cell that are not already listed under battery cell composition."
                },
                "language_tag": {
                  "$ref": "#/$defs/language_tag"
                }
              },
              "additionalProperties": false
            },
            "title": "Battery Cell Composition Other Than Listed",
            "examples": [
              "Silver Oxide"
            ],
            "minItems": 1,
            "selectors": [
              "language_tag"
            ],
            "description": "Provide the components of the item's battery cell that are not already listed under battery cell composition.",
            "maxUniqueItems": 1,
            "minUniqueItems": 1
          }
        },
        "additionalProperties": false
      },
      "title": "Battery",
      "examples": [
        "Alkaline"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide battery information",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "pattern": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Animal Print",
                  "Argyle",
                  "Camouflage",
                  "Checkered",
                  "Chevron",
                  "Floral",
                  "Geometric",
                  "Herringbone",
                  "Houndstooth",
                  "Moiré",
                  "Paisley",
                  "Plaid",
                  "Polka Dot",
                  "Solid",
                  "Striped",
                  "Toile"
                ],
                "type": "string",
                "enumNames": [
                  "Animal Print",
                  "Argyle",
                  "Camouflage",
                  "Checkered",
                  "Chevron",
                  "Floral",
                  "Geometric",
                  "Herringbone",
                  "Houndstooth",
                  "Moiré",
                  "Paisley",
                  "Plaid",
                  "Polka Dot",
                  "Solid",
                  "Striped",
                  "Toile"
                ]
              }
            ],
            "title": "Pattern",
            "hidden": false,
            "editable": true,
            "examples": [
              "Floral, Geometric, Polka Dot"
            ],
            "maxLength": 2200,
            "description": "Provide the most prominent repeated decorative design of the item",
            "maxUtf8ByteLength": 2000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Pattern",
      "examples": [
        "Floral, Geometric, Polka Dot"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide the most prominent repeated decorative design of the item",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "voltage": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "kilovolts",
              "microvolts",
              "millivolts",
              "nanovolts",
              "volts",
              "volts_of_alternating_current",
              "volts_of_direct_current"
            ],
            "type": "string",
            "title": "Voltage Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Volts"
            ],
            "enumNames": [
              "Kilovolts",
              "Microvolts",
              "Millivolts",
              "Nanovolts",
              "Volts",
              "Volts (AC)",
              "Volts (DC)"
            ],
            "description": "Select the unit of measure for Voltage. If a value is provided for Voltage, you must also enter the corresponding unit."
          },
          "value": {
            "type": "number",
            "title": "Voltage",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "28"
            ],
            "description": "Provide the voltage value as a numeric value"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Voltage",
      "examples": [
        "28 Volts"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the item's voltage",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "wattage": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "kilowatt_hours",
              "kilowatts",
              "microwatts",
              "milliamp_hours",
              "milliwatts",
              "nanowatts",
              "picowatts",
              "watt_hours",
              "watts"
            ],
            "type": "string",
            "title": "Wattage Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Watts"
            ],
            "enumNames": [
              "Kilowatt Hours",
              "Kilowatts",
              "Microwatts",
              "Milliamp Hours",
              "Milliwatts",
              "Nanowatts",
              "Picowatts",
              "Watt Hours",
              "Watts"
            ],
            "description": "Select the unit of measure for Wattage. If a value is provided for Wattage, you must also enter the corresponding unit."
          },
          "value": {
            "type": "number",
            "title": "Wattage",
            "hidden": false,
            "editable": true,
            "examples": [
              "50"
            ],
            "description": "Provide the wattage rating as a numeric value"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Wattage",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The wattage rating of the product. Input a number only--do not enter units.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "capacity": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "unit",
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "centiliters",
              "centiliters_per_second",
              "cubic_centimeters",
              "cubic_feet",
              "cubic_inches",
              "cubic_meters",
              "cubic_yards",
              "cups",
              "deciliters",
              "fluid_ounces",
              "gallons_per_day",
              "gallons",
              "grams",
              "hundredths_pounds",
              "imperial_gallons",
              "kilograms",
              "liters_per_day",
              "liters_per_second",
              "liters",
              "load",
              "liters_per_minute",
              "microliters",
              "microliters_per_minute",
              "microliters_per_second",
              "milligrams",
              "milliliters",
              "milliliters_per_second",
              "milliliters_per_minute",
              "nanoliters",
              "nanoliters_per_minute",
              "nanoliters_per_second",
              "ounces",
              "picoliters",
              "picoliters_per_minute",
              "picoliters_per_second",
              "pints",
              "pounds",
              "quarts",
              "tons"
            ],
            "type": "string",
            "title": "Capacity Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Cubic Centimetres, Cubic Feet"
            ],
            "enumNames": [
              "Centiliters",
              "Centiliters per Second",
              "Cubic Centimeters",
              "Cubic Feet",
              "Cubic Inches",
              "Cubic Meters",
              "Cubic Yards",
              "Cups",
              "Deciliters",
              "Fluid Ounces",
              "G/day",
              "Gallons",
              "Grams",
              "Hundredths Pounds",
              "Imperial Gallons",
              "Kilograms",
              "L/day",
              "L/sec",
              "Liters",
              "load",
              "LPM",
              "Microliters",
              "Microliters per Minute",
              "Microliters per Second",
              "Milligrams",
              "Milliliters",
              "Milliliters per Second",
              "ml/min",
              "Nanoliters",
              "Nanoliters per Minute",
              "Nanoliters per Second",
              "ounces",
              "Picoliters",
              "Picoliters per Minute",
              "Picoliters per Second",
              "Pints",
              "Pounds",
              "Quarts",
              "Tons"
            ],
            "description": "Select the unit of measure for Capacity. If a value is provided for Capacity, you must also enter the corresponding unit."
          },
          "value": {
            "type": "number",
            "title": "Capacity",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "5.3"
            ],
            "maxLength": 5000,
            "description": "Provide the capacity of the item as a numeric value"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Capacity",
      "examples": [
        "5.3"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The capacity of the item.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "material": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Acrylic",
                  "Acrylonitrile Butadiene Styrene",
                  "Alloy Steel",
                  "Aluminum",
                  "Beechwood",
                  "Brass",
                  "Carbon Steel",
                  "Cast Iron",
                  "Ceramic",
                  "Copper",
                  "Glass",
                  "Granite",
                  "Iron",
                  "Marble",
                  "Metal",
                  "Oak",
                  "Olivewood",
                  "Pine Wood",
                  "Plastic",
                  "Polycarbonate",
                  "Polypropylene",
                  "Porcelain",
                  "Resin",
                  "Rubber",
                  "Rubberwood",
                  "Silicone",
                  "Stainless Steel",
                  "Stone",
                  "Thermoplastic Elastomers",
                  "Walnut",
                  "Wood",
                  "Zinc"
                ],
                "type": "string",
                "enumNames": [
                  "Acrylic",
                  "Acrylonitrile Butadiene Styrene",
                  "Alloy Steel",
                  "Aluminum",
                  "Beechwood",
                  "Brass",
                  "Carbon Steel",
                  "Cast Iron",
                  "Ceramic",
                  "Copper",
                  "Glass",
                  "Granite",
                  "Iron",
                  "Marble",
                  "Metal",
                  "Oak",
                  "Olivewood",
                  "Pine Wood",
                  "Plastic",
                  "Polycarbonate",
                  "Polypropylene",
                  "Porcelain",
                  "Resin",
                  "Rubber",
                  "Rubberwood",
                  "Silicone",
                  "Stainless Steel",
                  "Stone",
                  "Thermoplastic Elastomers",
                  "Walnut",
                  "Wood",
                  "Zinc"
                ]
              }
            ],
            "title": "Material",
            "hidden": false,
            "editable": true,
            "examples": [
              "18/8 Stainless Steel, 18/10 Steel"
            ],
            "description": "Specify the primary materials used for manufacturing the item",
            "maxUtf8ByteLength": 2000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Material Type",
      "examples": [
        "nylon, wood, steel"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "What material is the product made out of?",
      "maxUniqueItems": 14,
      "minUniqueItems": 1
    },
    "item_name": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Item Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "Adidas Blue Sneakers"
            ],
            "maxLength": 200,
            "minLength": 0,
            "description": "Provide a title for the item that may be customer facing"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Title",
      "examples": [
        "Adidas Blue Sneakers"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide a title for the item that may be customer facing",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "team_name": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "1. FC Koln",
                  "1. FC Magdeburg",
                  "A. J. Allmendinger",
                  "A.S. Livorno Calcio",
                  "Aberdeen",
                  "Aberdeen IronBirds",
                  "Abilene Christian Wildcats",
                  "AC Ajaccio",
                  "AC Milan",
                  "AC Nagano Parceiro",
                  "AD Alcorcón",
                  "ADO Den Haag",
                  "AFC Bournemouth",
                  "Afghanistan",
                  "Ahmedabad Defenders",
                  "Air Force Falcons",
                  "Airdrieonians",
                  "AISIN AW AREIONS ANJO",
                  "Aizawl FC",
                  "Ajax Amsterdam",
                  "AKITA NORTHERN HAPPINETS",
                  "Akron Aeros",
                  "Akron Zips",
                  "Al Iaquinta",
                  "Alabama A&M Bulldogs",
                  "Alabama Birmingham Blazers",
                  "Alabama Crimson Tide",
                  "Alabama State Hornets",
                  "Alaves",
                  "ALBA Berlin Basketball",
                  "Albacete BP",
                  "Albania",
                  "Albany Great Danes",
                  "Albirex Niigata",
                  "Albuquerque Isotopes",
                  "Alcorn State Braves",
                  "Alejandro Perez",
                  "Alex Bowman",
                  "Alex Oliveira",
                  "Alex Perez",
                  "Alexa Grasso",
                  "Alexander Gustafsson",
                  "Alexander Hernandez",
                  "Alexander Volkanoski",
                  "Alexander Volkov",
                  "Alexandre Pantoja",
                  "Alexis Davis",
                  "Alfa Romeo Racing",
                  "Algeria",
                  "Alistair Overeem",
                  "Aljamain Sterling",
                  "Almere City",
                  "Alpine",
                  "Altoona Curve",
                  "ALVARK TOKYO",
                  "Amanda Nunes",
                  "American Samoa",
                  "American University Eagles",
                  "Amiens SC",
                  "Anadolu Efes Istanbul Basketball",
                  "Anaheim Ducks",
                  "Andorra",
                  "Andrea Lee",
                  "Andrei Arlovski",
                  "Angel City FC",
                  "Angela Hill",
                  "Angers SCO",
                  "Angola",
                  "Anthony Pettis",
                  "Anthony Smith",
                  "Antigua and Barbuda",
                  "Antonio Carlos Junior",
                  "AOMORI WAT'S",
                  "Appalachian State Mountaineers",
                  "Arbroath",
                  "Argentina",
                  "Aric Almirola",
                  "Arizona Cardinals",
                  "Arizona Coyotes",
                  "Arizona Diamondbacks",
                  "Arizona State Sun Devils",
                  "Arizona Wildcats",
                  "Arkansas Little Rock Trojans",
                  "Arkansas Razorbacks",
                  "Arkansas State Indians",
                  "Arkansas State Red Wolves",
                  "Arkansas Travelers",
                  "Arkansas-Pine Bluff Golden Lions",
                  "Armenia",
                  "Arminia Bielefeld",
                  "Army Black Knights",
                  "Arsenal",
                  "Arsenal de Sarandí",
                  "Aruba",
                  "AS Roma",
                  "AS Saint-Etienne",
                  "Ascoli",
                  "Asheville Tourists",
                  "Ashlee Evans-Smith",
                  "Aspen Ladd",
                  "Aston Martin",
                  "Aston Villa",
                  "Atalanta",
                  "Athletic Bilbao",
                  "ATK Mohun Bagan FC",
                  "Atlanta Braves",
                  "Atlanta Dream",
                  "Atlanta Falcons",
                  "Atlanta Flames",
                  "Atlanta Hawks",
                  "Atlanta Thrashers",
                  "Atlanta United FC",
                  "Atletico Madrid",
                  "Atlético de San Luis",
                  "Atlético Ottawa",
                  "Auburn Doubledays",
                  "Auburn Tigers",
                  "Augusta GreenJackets",
                  "Austin Dillon",
                  "Austin FC",
                  "Austin Peay Governors",
                  "Australia",
                  "Austria",
                  "Auxerre",
                  "Avispa Fukuoka",
                  "Awadhe Warriors",
                  "AX Armani Exchange Milan Basketball",
                  "AZ Alkmaar",
                  "Azerbaijan",
                  "Bahamas",
                  "Bahrain",
                  "Bakersfield Blaze",
                  "Ball State Cardinals",
                  "Baltimore Orioles",
                  "Baltimore Ravens",
                  "BAMBITIOUS NARA",
                  "Bangladesh",
                  "Barbados",
                  "Barcelona",
                  "Barcelona Basketball",
                  "Bari",
                  "Bastia",
                  "Batavia Muckdogs",
                  "Bates Bobcats",
                  "Bayer Leverkusen",
                  "Bayern Munich",
                  "Bayern Munich Basketball",
                  "Baylor Bears",
                  "BC Lions",
                  "Belarus",
                  "Belenenses",
                  "Belgium",
                  "Belize",
                  "Belmont Bruins",
                  "Beloit Snappers",
                  "Ben Nguyen",
                  "Benfica",
                  "Bengal Warriors",
                  "Bengaluru Bulls",
                  "Bengaluru FC",
                  "Bengaluru Raptors",
                  "Benin",
                  "Bermuda",
                  "Bethe Correia",
                  "Bethune Cookman Wildcats",
                  "Betis Sevilla",
                  "Bhutan",
                  "Billings Mustangs",
                  "Binghamton Bearcats",
                  "Binghamton Mets",
                  "Birmingham Barons",
                  "Birmingham City",
                  "Black Hawks Hyderabad",
                  "Blackburn Rovers",
                  "Blaublitz Akita",
                  "Bluefield Orioles",
                  "Boavista",
                  "Bobby Labonte",
                  "Boca Juniors",
                  "Boise Hawks",
                  "Boise State Broncos",
                  "Bolivia",
                  "Bologna",
                  "Bolton Wanderers",
                  "Bordeaux",
                  "Borussia Dortmund",
                  "Borussia Monchengladbach",
                  "Bosnia and Herzegovina",
                  "Boston Beaneaters",
                  "Boston Beans",
                  "Boston Bruins",
                  "Boston Celtics",
                  "Boston College Eagles",
                  "Boston Legacy FC",
                  "Boston Patriots",
                  "Boston Red Sox",
                  "Boston Redskins",
                  "Boston University Terriers",
                  "Botswana",
                  "Bowie Baysox",
                  "Bowling Green Falcons",
                  "Bowling Green Hot Rods",
                  "Brad Keselowski",
                  "Brad Tavares",
                  "Bradenton Marauders",
                  "Bradley Braves",
                  "Brandon Moreno",
                  "Brazil",
                  "Brentford",
                  "Brescia",
                  "Brest",
                  "Brevard County Manatees",
                  "Brian Ortega",
                  "Brighton & Hove Albion",
                  "Bristol City",
                  "Bristol White Sox",
                  "British Virgin Islands",
                  "Brooklyn Cyclones",
                  "Brooklyn Nets",
                  "Brown Bears",
                  "Brunei",
                  "Bryant Bulldogs",
                  "Bucknell Bison",
                  "Buffalo Bandits",
                  "Buffalo Bills",
                  "Buffalo Bisons",
                  "Buffalo Braves",
                  "Buffalo Bulls",
                  "Buffalo Sabres",
                  "Bulgaria",
                  "Burkina Faso",
                  "Burlington Bees",
                  "Burlington Royals",
                  "Burnley",
                  "Burundi",
                  "Butler Bulldogs",
                  "BWT Racing Point",
                  "BYU Cougars",
                  "C.D. Chivas USA",
                  "CA River Plate",
                  "Cagliari Calcio",
                  "Cal Irvine Anteaters",
                  "Cal Poly Mustangs",
                  "Cal Riverside Highlanders",
                  "Cal Santa Barbara Gauchos",
                  "Cal State Bakersfield Roadrunners",
                  "Cal State Fullerton Titans",
                  "Cal State Northridge Matadors",
                  "Cal State Sacramento Hornets",
                  "Calcio Catania",
                  "Calgary Flames",
                  "Calgary Roughnecks",
                  "Calgary Stampeders",
                  "Calicut Heroes",
                  "California Angels",
                  "California Baptist Lancers",
                  "California Golden Bears",
                  "California Seals",
                  "Cambodia",
                  "Cameroon",
                  "Campbell Fighting Camels",
                  "Canada",
                  "Canisius Golden Griffins",
                  "Cape Verde",
                  "Cardiff City",
                  "Carl Edwards",
                  "Carla Esparza",
                  "Carolina Hurricanes",
                  "Carolina Mudcats",
                  "Carolina Panthers",
                  "Casa Pia AC",
                  "Casey Mears",
                  "Casper Ghosts",
                  "Cat Zingano",
                  "Catanzaro",
                  "Cavalry FC",
                  "Cayman Islands",
                  "CD Lugo",
                  "CD Mirandés",
                  "CD Numancia",
                  "CD Santa Clara",
                  "CD Tenerife",
                  "Cedar Rapids Kernels",
                  "Celta Vigo",
                  "Celtic",
                  "Centenary Gentlemen",
                  "Central African Republic",
                  "Central Arkansas Bears",
                  "Central Connecticut Blue Devils",
                  "Central Connecticut State Blue Devils",
                  "Central Florida Golden Knights",
                  "Central Michigan Chippewas",
                  "Cerezo Osaka",
                  "CF Atlas",
                  "CF Estrela",
                  "CF Fuenlabrada",
                  "CF Monterrey",
                  "Chad",
                  "Chad Mendes",
                  "Chan Sung Jung",
                  "Charleston Cougars",
                  "Charleston RiverDogs",
                  "Charleston Southern Buccaneers",
                  "Charlotte 49ers",
                  "Charlotte Hornets",
                  "Charlotte Knights",
                  "Charlotte Sting",
                  "Charlotte Stone Crabs",
                  "Charlton Athletic",
                  "Chase Elliott",
                  "Chattanooga Lookouts",
                  "Chaves",
                  "Chelsea",
                  "Chennai City FC",
                  "Chennai Spartans",
                  "Chennai Super Kings",
                  "Chennai Superstarz",
                  "Chennaiyin FC",
                  "CHIBA JETS",
                  "Chiba Lotte Marines",
                  "Chicago Bears",
                  "Chicago Blackhawks",
                  "Chicago Bulls",
                  "Chicago Cardinals",
                  "Chicago Cubs",
                  "Chicago Fire",
                  "Chicago Red Stars",
                  "Chicago Sky",
                  "Chicago Stags",
                  "Chicago State Cougars",
                  "Chicago White Sox",
                  "Chicago White Stockings",
                  "Chicago Whitesox",
                  "Chicago Zephyrs",
                  "Chievo Verona",
                  "Chile",
                  "China",
                  "Chinese Taipei",
                  "Chris Buescher",
                  "Chris Weidman",
                  "Chunichi Dragons",
                  "Churchill Brothers FC Goa",
                  "Cincinnati Bearcats",
                  "Cincinnati Bengals",
                  "Cincinnati Redlegs",
                  "Cincinnati Reds",
                  "Citadel Bulldogs",
                  "Cittadella",
                  "Claudia Gadelha",
                  "Clearwater Threshers",
                  "Clemson Tigers",
                  "Clermont Foot 63",
                  "Cleveland Barons",
                  "Cleveland Blues",
                  "Cleveland Browns",
                  "Cleveland Cavaliers",
                  "Cleveland Indians",
                  "Cleveland Naps",
                  "Cleveland Rockers",
                  "Cleveland State Vikings",
                  "Clint Bowyer",
                  "Clinton LumberKings",
                  "Club América",
                  "Club Atlético River Plate",
                  "Club Deportivo Guadalajara - Chivas",
                  "Club Deportivo Social y Cultural - Cruz Azul",
                  "Club Santos Laguna",
                  "Club Universidad Nacional A.C. - Pumas",
                  "Coastal Carolina Chanticleers",
                  "Cody Garbrandt",
                  "Cody Stamann",
                  "Colby Covington",
                  "Colgate Raiders",
                  "Colombia",
                  "Colorado Avalanche",
                  "Colorado Buffaloes",
                  "Colorado College Tigers",
                  "Colorado Mammoth",
                  "Colorado Rapids",
                  "Colorado Rockies",
                  "Colorado Springs Sky Sox",
                  "Colorado State Rams",
                  "Columbia Lions",
                  "Columbus Blue Jackets",
                  "Columbus Clippers",
                  "Columbus Crew",
                  "Como",
                  "Comoros",
                  "Congo",
                  "Connecticut Huskies",
                  "Connecticut Sun",
                  "Connecticut Tigers",
                  "Conor McGregor",
                  "Consadole Sapporo",
                  "Cook Islands",
                  "Coppin State Eagles",
                  "Corey Anderson",
                  "Cornell Big Red",
                  "Corpus Christi Hooks",
                  "Cortney Casey",
                  "Cosenza",
                  "Costa Rica",
                  "Cote d'Ivoire",
                  "Coventry City",
                  "Creighton Bluejays",
                  "Cris Cyborg",
                  "Croatia",
                  "Crvena Zvezda mts Belgrade Basketball",
                  "Crystal Palace",
                  "CSKA Moscow Basketball",
                  "Cub Swanson",
                  "Cuba",
                  "Curtis Blaydes",
                  "Cyprus",
                  "Czech Republic",
                  "Cádiz CF",
                  "D.C. United",
                  "Dabang Delhi KC",
                  "Dabang Mumbai HC",
                  "Dale Earnhardt",
                  "Dale Earnhardt Jr.",
                  "Dallas Baptist Patriots",
                  "Dallas Cowboys",
                  "Dallas Mavericks",
                  "Dallas Stars",
                  "Dallas Texans",
                  "Dallas Wings",
                  "Dan Hooker",
                  "Daniel Cormier",
                  "Daniel Suárez",
                  "Danville Braves",
                  "Darmstadt 98",
                  "Darrell Wallace Jr.",
                  "Darren Elkins",
                  "Darren Till",
                  "Dartmouth Big Green",
                  "David Branch",
                  "David Ragan",
                  "Davidson Wildcats",
                  "Dayton Dragons",
                  "Dayton Flyers",
                  "Daytona Cubs",
                  "De Graafschap",
                  "Deiveson Figueiredo",
                  "Delaware Fightin' Blue Hens",
                  "Delaware State Hornets",
                  "Delhi Capitals",
                  "Delhi Sultans",
                  "Delhi Waveriders",
                  "Delmarva Shorebirds",
                  "Demian Maia",
                  "Democratic Republic of the Congo",
                  "Denmark",
                  "Denny Hamlin",
                  "Denver Broncos",
                  "Denver Nuggets",
                  "Denver Pioneers",
                  "DePaul Blue Demons",
                  "Deportivo La Coruna",
                  "Derby County",
                  "Derek Brunson",
                  "Derrick Lewis",
                  "Desportivo das Aves",
                  "Detroit Cougars",
                  "Detroit Falcons",
                  "Detroit Lions",
                  "Detroit Pistons",
                  "Detroit Red Wings",
                  "Detroit Shock",
                  "Detroit Tigers",
                  "Detroit Titans",
                  "Dijon FCO",
                  "Djibouti",
                  "Dominica",
                  "Dominican Republic",
                  "Dominick Cruz",
                  "Dominick Reyes",
                  "Donald Cerrone",
                  "Douglas Silva de Andrade",
                  "Drake Bulldogs",
                  "Drexel Dragons",
                  "Duke Blue Devils",
                  "Dundee",
                  "Dundee United",
                  "Dunedin Blue Jays",
                  "Dunfermline",
                  "Duquesne Dukes",
                  "Durham Bulls",
                  "Dustin Ortiz",
                  "Dustin Poirier",
                  "Dynamo Dresden",
                  "E-Sports",
                  "EARTHFRIENDS TOKYO Z",
                  "East Carolina Pirates",
                  "East Tennessee State Buccaneers",
                  "East Timor",
                  "Eastern Illinois Panthers",
                  "Eastern Kentucky Colonels",
                  "Eastern Michigan Eagles",
                  "Eastern Washington Eagles",
                  "Ecuador",
                  "Edmonton Football Team",
                  "Edmonton Oilers",
                  "Edson Barboza",
                  "Egypt",
                  "Ehime FC",
                  "EHIME ORANGE VIKINGS",
                  "Eintracht Braunschweig",
                  "Eintracht Frankfurt",
                  "El Salvador",
                  "Elche CF",
                  "Elias Theodorou",
                  "Elizabethton Twins",
                  "Elizeu Zaleski dos Santos",
                  "Elliott Sadler",
                  "Elon Phoenix",
                  "Empoli",
                  "Energie Cottbus",
                  "England",
                  "Equatorial Guinea",
                  "Erie SeaWolves",
                  "Erik Jones",
                  "Eritrea",
                  "Espanyol",
                  "Estonia",
                  "Estoril",
                  "Ethiopia",
                  "Eugene Emeralds",
                  "Evansville Purple Aces",
                  "Everett AquaSox",
                  "Everton",
                  "Excelsior",
                  "Extremadura UD",
                  "F EAGLES NAGOYA",
                  "F.C. Gifu",
                  "Fagiano Okayama FC",
                  "Fairfield Stags",
                  "Fairleigh Dickinson Devils",
                  "Fairleigh Dickinson Knights",
                  "Famalicão",
                  "Farense",
                  "FC Arouca",
                  "FC Arsenal Tula",
                  "FC Augsburg",
                  "FC Basel",
                  "FC Cincinnati",
                  "FC Dallas",
                  "FC Edmonton",
                  "FC Goa",
                  "FC Groningen",
                  "FC Heidenheim",
                  "FC Juárez",
                  "FC Lorient",
                  "FC Machida Zelvia",
                  "FC Ryūkyū",
                  "FC Sevilla",
                  "FC St. Pauli",
                  "FC Startak Moscow",
                  "FC Tokyo",
                  "FC Utrecht",
                  "FC Volendam",
                  "FC Zwolle",
                  "Federated States of Micronesia",
                  "Felice Herrig",
                  "Fenerbahce Beko Istanbul",
                  "Feyenoord Rotterdam",
                  "Fiji",
                  "Finland",
                  "Fiorentina",
                  "FIU Panthers",
                  "Florida A&M Rattlers",
                  "Florida Atlantic Owls",
                  "Florida Gators",
                  "Florida Gulf Coast Eagles",
                  "Florida International Golden Panthers",
                  "Florida Panthers",
                  "Florida State Seminoles",
                  "Fordham Rams",
                  "Forge FC",
                  "Fort Myers Miracle",
                  "Fort Wayne Mastodons",
                  "Fort Wayne Pistons",
                  "Fort Wayne TinCaps",
                  "Fortuna Düsseldorf",
                  "Fortuna Sittard",
                  "France",
                  "Francis Ngannou",
                  "Francisco Trinaldo",
                  "Frankie Edgar",
                  "Frederick Keys",
                  "Fresno Grizzlies",
                  "Fresno State Bulldogs",
                  "Frisco RoughRiders",
                  "Frosinone FC",
                  "FSV Mainz 05",
                  "Fujieda MYFC",
                  "Fukuoka SoftBank Hawks",
                  "FUKUSHIMA FIREBONDS",
                  "Fukushima United FC",
                  "Fulham",
                  "Furman Paladins",
                  "Gabon",
                  "Gainare Tottori",
                  "Galatasaray SK",
                  "Gamba Osaka",
                  "Gardner-Webb Runnin' Bulldogs",
                  "Genoa",
                  "George Mason Patriots",
                  "George Washington Colonials",
                  "Georges St-Pierre",
                  "Georgetown Hoyas",
                  "Georgia",
                  "Georgia Bulldogs",
                  "Georgia Southern Eagles",
                  "Georgia State Panthers",
                  "Georgia Swarm",
                  "Georgia Tech Yellow Jackets",
                  "Germaine de Randamie",
                  "Germany",
                  "Getafe CF",
                  "Getafe FC",
                  "Ghana",
                  "Gil Vicente",
                  "Giravanz Kitakyushu",
                  "Girona FC",
                  "Glover Teixeira",
                  "Go Ahead Eagles",
                  "Gokulam Kerala FC",
                  "Golden State Valkyries",
                  "Golden State Warriors",
                  "Gonzaga Bulldogs",
                  "Grambling Tigers",
                  "Granada CF",
                  "Grand Canyon Antelopes",
                  "Gray Gaulding",
                  "Great Britain",
                  "Great Falls Voyagers",
                  "Great Lakes Loons",
                  "Greece",
                  "Green Bay Packers",
                  "Greeneville Astros",
                  "Greensboro Grasshoppers",
                  "Greenville Drive",
                  "Greg Biffle",
                  "Grenada",
                  "Greuther Fürth",
                  "Grulla Morioka",
                  "Guam",
                  "Guatemala",
                  "Guinea",
                  "Guinea-Bissau",
                  "Guingamp",
                  "Gujarat Fortunegiants",
                  "Gujarat Lions",
                  "GUNMA CRANE THUNDERS",
                  "Gunnar Nelson",
                  "Guyana",
                  "Gwinnett Braves",
                  "Haas F1 Team",
                  "Hagerstown Suns",
                  "Haiti",
                  "Halifax Thunderbirds",
                  "Hamburg SV",
                  "Hamilton Tiger-Cats",
                  "Hamilton Tigers",
                  "Hampton Pirates",
                  "Hannover 96",
                  "Hansa Rostock",
                  "Hanshin Tigers",
                  "Harrisburg Senators",
                  "Hartford Hawks",
                  "Hartford Whalers",
                  "Harvard Crimson",
                  "Haryana Hammers",
                  "Haryana Steelers",
                  "Hawaii Rainbow Warriors",
                  "Hearts",
                  "Heerenveen",
                  "Helena Brewers",
                  "Henry Cejudo",
                  "Heracles Almelo",
                  "Hertha Berlin",
                  "Hertha BSC",
                  "HFX Wanderers FC",
                  "Hibernian",
                  "Hickory Crawdads",
                  "High Desert Mavericks",
                  "High Point Panthers",
                  "High School Baseball Team",
                  "HIROSHIMA DRAGONFLIES",
                  "Hiroshima Toyo Carp",
                  "Hofstra Flying Dutchmen",
                  "Hofstra Pride",
                  "Hokkaido Nippon-Ham Fighters",
                  "Holly Holm",
                  "Holy Cross Crusaders",
                  "Honduras",
                  "Hong Kong",
                  "Houston Astros",
                  "Houston Baptist Huskies",
                  "Houston Comets",
                  "Houston Cougars",
                  "Houston Dash",
                  "Houston Dynamo",
                  "Houston Oilers",
                  "Houston Rockets",
                  "Houston Texans",
                  "Howard Bison",
                  "Huddersfield Town",
                  "Hudson Valley Renegades",
                  "Hull City",
                  "Hungary",
                  "Huntsville Stars",
                  "Hyderabad FC",
                  "Hyderabad Hunters",
                  "IBARAKI ROBOTS",
                  "Iceland",
                  "Idaho Falls Chukars",
                  "Idaho State Bengals",
                  "Idaho Vandals",
                  "Ilir Latifi",
                  "Illinois Chicago Flames",
                  "Illinois Illini",
                  "Illinois State Redbirds",
                  "Incarnate Word Cardinals",
                  "Independent Olympic Athletes",
                  "India",
                  "Indian Arrows",
                  "Indiana Fever",
                  "Indiana Hoosiers",
                  "Indiana Pacers",
                  "Indiana State Sycamores",
                  "Indianapolis Colts",
                  "Indianapolis Indians",
                  "Indonesia",
                  "Inland Empire 66ers",
                  "Inter Miami CF",
                  "Inter Milan",
                  "Inverness Caledonian Thistle",
                  "Iona Gaels",
                  "Iowa Cubs",
                  "Iowa Hawkeyes",
                  "Iowa State Cyclones",
                  "IPFW Mastodons",
                  "Ipswich Town",
                  "Iran",
                  "Iraq",
                  "Ireland",
                  "Irene Aldana",
                  "Israel",
                  "Israel Adesanya",
                  "Italy",
                  "IUPUI Jaguars",
                  "Ivory Coast",
                  "Iwaki FC",
                  "IWATE BIG BULLS",
                  "Jacare Souza",
                  "Jackson State Tigers",
                  "Jacksonville Dolphins",
                  "Jacksonville Jaguars",
                  "Jacksonville State Gamecocks",
                  "Jacksonville Suns",
                  "Jaipur Pink Panthers",
                  "Jamaica",
                  "James Madison Dukes",
                  "James Vick",
                  "Jamestown Jammers",
                  "Jamie McMurray",
                  "Jamshedpur FC",
                  "Jan Blachowicz",
                  "Japan",
                  "Jared Cannonier",
                  "Jaypee Punjab Warriors",
                  "JEF United Ichihara Chiba",
                  "Jeff Burton",
                  "Jeff Gordon",
                  "Jennifer Maia",
                  "Jeremy Stephens",
                  "Jessica Andrade",
                  "Jessica Eye",
                  "Jessica-Rose Clark",
                  "Jimi Manuwa",
                  "Jimmie Johnson",
                  "Jimmie Rivera",
                  "Joanna Jedrzejczyk",
                  "Joanne Calderwood",
                  "Joey Logano",
                  "John Dodson",
                  "John Lineker",
                  "John Moraga",
                  "Johnson City Cardinals",
                  "Jon Jones",
                  "Jordan",
                  "Jorge Masvidal",
                  "Jose Aldo",
                  "Joseph Benavidez",
                  "Josh Emmett",
                  "Juan Pablo Montoya",
                  "Julianna Pena",
                  "Junior dos Santos",
                  "Jupiter Hammerheads",
                  "Jussier Formiga",
                  "Justin Gaethje",
                  "Justin Willis",
                  "Juventus",
                  "Júbilo Iwata",
                  "KAGAWA FIVE ARROWS",
                  "KAGOSHIMA REBNISE",
                  "Kaiserslautern",
                  "Kalinga Lancers",
                  "Kamaru Usman",
                  "Kamatamare Sanuki",
                  "KANAZAWA SAMURAIZ",
                  "Kane County Cougars",
                  "Kannapolis Intimidators",
                  "Kansas City Athletics",
                  "Kansas City Chiefs",
                  "Kansas City Current",
                  "Kansas City Kings",
                  "Kansas City Royals",
                  "Kansas City Scouts",
                  "Kansas Jayhawks",
                  "Kansas State Wildcats",
                  "Karlsruher SC",
                  "Karolina Kowalkiewicz",
                  "Kasey Kahne",
                  "Kashima Antlers",
                  "Kashiwa Reysol",
                  "Kataller Toyama",
                  "Katlyn Chookagian",
                  "KAWASAKI BRAVE THUNDERS",
                  "Kawasaki Frontale",
                  "Kazakhstan",
                  "Kelvin Gastelum",
                  "Kennesaw State Owls",
                  "Kent State Golden Flashes",
                  "Kentucky Wildcats",
                  "Kenya",
                  "Kerala Blasters FC",
                  "Ketlen Vieira",
                  "Kevin Harvick",
                  "Kevin Lee",
                  "Khabib Nurmagomedov",
                  "Khimki Moscow Region Basketball",
                  "Kilmarnock",
                  "Kings XI Punjab",
                  "Kingsport Mets",
                  "Kinston Indians",
                  "Kiribati",
                  "KIROLBET Baskonia Vitoria-Gasteiz Basketball",
                  "Kochi Blue Spikers",
                  "Kolkata Knight Riders",
                  "Kosovo",
                  "KUMAMOTO VOLTERS",
                  "Kurt Busch",
                  "Kyle Busch",
                  "Kyle Larson",
                  "KYOTO HANNARYZ",
                  "Kyoto Sanga FC",
                  "Kyrgyzstan",
                  "La Salle Explorers",
                  "Lafayette Leopards",
                  "Lake County Captains",
                  "Lake Elsinore Storm",
                  "Lakeland Flying Tigers",
                  "Lakewood BlueClaws",
                  "Lamar Cardinals",
                  "Lancaster JetHawks",
                  "Lansing Lugnuts",
                  "Laos",
                  "Las Vegas 51s",
                  "Las Vegas Aces",
                  "Las Vegas Raiders",
                  "Latvia",
                  "Lauren Murphy Increase1",
                  "Lazio",
                  "LDLC ASVEL Villeurbanne",
                  "Le Havre",
                  "Lebanon",
                  "Lecce",
                  "Lecco",
                  "Leeds United",
                  "Leganés",
                  "Lehigh Mountain Hawks",
                  "Lehigh Valley IronPigs",
                  "Leicester City",
                  "Lens",
                  "Leon Edwards",
                  "Lesotho",
                  "LEVANGA HOKKAIDO",
                  "Levante UD",
                  "Lexington Legends",
                  "Liberia",
                  "Liberty Flames",
                  "Libya",
                  "Liechtenstein",
                  "Lille",
                  "Lina Lansberg",
                  "Lipscomb Bisons",
                  "Lithuania",
                  "Liverpool",
                  "Livingston",
                  "Liz Carmouche",
                  "Long Beach State 49ers",
                  "Long Beach State Sharks",
                  "Long Island Blackbirds",
                  "Longwood Lancers",
                  "Los Angeles Angels",
                  "Los Angeles Chargers",
                  "Los Angeles Clippers",
                  "Los Angeles Dodgers",
                  "Los Angeles FC",
                  "Los Angeles Galaxy",
                  "Los Angeles Kings",
                  "Los Angeles Lakers",
                  "Los Angeles Rams",
                  "Los Angeles Sparks",
                  "Louisiana Lafayette Ragin' Cajuns",
                  "Louisiana Monroe Indians",
                  "Louisiana Tech Bulldogs",
                  "Louisiana-Monroe Warhawks",
                  "Louisville Bats",
                  "Louisville Cardinals",
                  "Lowell Spinners",
                  "Loyola Chicago Ramblers",
                  "Loyola Maryland Greyhounds",
                  "Loyola Marymount Lions",
                  "LPGA",
                  "LSU Tigers",
                  "Lucie Pudilova",
                  "Luke Rockhold",
                  "Luton Town",
                  "Luxembourg",
                  "Lynchburg Hillcats",
                  "Lyon",
                  "Maccabi FOX Tel Aviv Basketball",
                  "Macedonia",
                  "Mackenzie Dern",
                  "Madagascar",
                  "Mahoning Valley Scrappers",
                  "Maine Black Bears",
                  "Malaga",
                  "Malawi",
                  "Malaysia",
                  "Maldives",
                  "Mali",
                  "Mallorca",
                  "Malta",
                  "Manchester City",
                  "Manchester United",
                  "Manhattan Jaspers",
                  "Mara Romero Borella",
                  "Marcin Tybura",
                  "Marion Reneau",
                  "Marist Red Foxes",
                  "Mark Hunt",
                  "Mark Martin",
                  "Marlon Moraes",
                  "Marquette Golden Eagles",
                  "Marseille",
                  "Marshall Islands",
                  "Marshall Thundering Herd",
                  "Martin Truex Jr.",
                  "Maryland Baltimore County Retrievers",
                  "Maryland Eastern Shore Fighting Hawks",
                  "Maryland Terrapins",
                  "Marítimo",
                  "Massachusetts Minutemen",
                  "Matheus Nicolau",
                  "Matsumoto Yamaga FC",
                  "Matt DiBenedetto",
                  "Matt Kenseth",
                  "Mauricio Rua",
                  "Mauritania",
                  "Mauritius",
                  "Max Holloway",
                  "Mazatlán",
                  "Mclaren",
                  "McNeese State Cowboys",
                  "Memphis Grizzlies",
                  "Memphis Redbirds",
                  "Memphis Tigers",
                  "Mercedes-AMG Petronas",
                  "Mercer Bears",
                  "Metz",
                  "Mexico",
                  "Miami (Ohio) Redhawks",
                  "Miami Dolphins",
                  "Miami Heat",
                  "Miami Hurricanes",
                  "Miami Marlins",
                  "Miami Sol",
                  "Michael Chiesa",
                  "Michael McDowell",
                  "Michelle Waterson",
                  "Michigan State Spartans",
                  "Michigan Wolverines",
                  "Middle Tennessee State Blue Raiders",
                  "Middlesbrough",
                  "Middleweight",
                  "Midland RockHounds",
                  "Millwall",
                  "Milwaukee Braves",
                  "Milwaukee Brewers",
                  "Milwaukee Bucks",
                  "Milwaukee Hawks",
                  "Minnesota Golden Gophers",
                  "Minnesota Lynx",
                  "Minnesota North Stars",
                  "Minnesota Timberwolves",
                  "Minnesota Twins",
                  "Minnesota United FC",
                  "Minnesota Vikings",
                  "Minnesota Wild",
                  "Mirsad Bektic",
                  "Misha Cirkunov",
                  "Mississippi Braves",
                  "Mississippi Old Miss Rebels",
                  "Mississippi State Bulldogs",
                  "Mississippi Valley State Delta Devils",
                  "Missoula Osprey",
                  "Missouri Kansas City Kangaroos",
                  "Missouri Tigers",
                  "Mito HollyHock",
                  "Mobile BayBears",
                  "Modena",
                  "Modesto Nuts",
                  "Mohun Bagan",
                  "Moldova",
                  "Monaco",
                  "Mongolia",
                  "Monmouth Hawks",
                  "Montana Grizzlies",
                  "Montana State Bobcats",
                  "Montedio Yamagata",
                  "Montenegro",
                  "Montgomery Biscuits",
                  "Montpellier",
                  "Montreal Alouettes",
                  "Montreal Canadiens",
                  "Montreal Expos",
                  "Montreal Impact",
                  "Montreal Maroons",
                  "Montreal Wanderers",
                  "Monza",
                  "Morehead State Eagles",
                  "Moreirense",
                  "Morgan State Bears",
                  "Morocco",
                  "Motherwell",
                  "Mount St. Mary's Mountaineers",
                  "Mozambique",
                  "MP Yodha",
                  "Mumbai City FC",
                  "Mumbai Indians",
                  "Mumbai Maharathi",
                  "Mumbai Rockets",
                  "Murray State Racers",
                  "Myanmar",
                  "Myrtle Beach Pelicans",
                  "NAC Breda",
                  "NAGOYA DIAMOND DOLPHINS",
                  "Nagoya Grampus Eight",
                  "Namibia",
                  "Nantes",
                  "Nashville Predators",
                  "Nashville SC",
                  "Nashville Sounds",
                  "Nate Diaz",
                  "Nauru",
                  "Navy Midshipmen",
                  "NCR Punjab Royals",
                  "Nebraska Cornhuskers",
                  "NEC Nijmegen",
                  "Necaxa",
                  "Neil Magny",
                  "Nepal",
                  "NEROCA FC",
                  "Netherlands",
                  "Nevada Wolf Pack",
                  "New Britain Rock Cats",
                  "New England Black Wolves",
                  "New England Patriots",
                  "New England Revolution",
                  "New Hampshire Fisher Cats",
                  "New Hampshire Wildcats",
                  "New Jersey Devils",
                  "New Jersey Nets",
                  "New Mexico Lobos",
                  "New Mexico State Aggies",
                  "New Orleans Pelicans",
                  "New Orleans Privateers",
                  "New Orleans Saints",
                  "New Orleans Zephyrs",
                  "New York Americans",
                  "New York City FC",
                  "New York Giants",
                  "New York Highlanders",
                  "New York Islanders",
                  "New York Jets",
                  "New York Knicks",
                  "New York Liberty",
                  "New York Mets",
                  "New York Rangers",
                  "New York Red Bulls",
                  "New York Riptide",
                  "New York Titans",
                  "New York Yankees",
                  "New Zealand",
                  "Newcastle United",
                  "Niagara Purple Eagles",
                  "Nicaragua",
                  "Nicco Montaño",
                  "Nice",
                  "Nicholls State Colonels",
                  "Niger",
                  "Nigeria",
                  "NIIGATA ALBIREX BB",
                  "Nikita Krylov",
                  "Nina Ansaroff",
                  "NISHINOMIYA STORKS",
                  "NJ/NY Gotham FC",
                  "NJIT Highlanders",
                  "Norfolk State Spartans",
                  "Norfolk Tides",
                  "North Alabama Lions",
                  "North Carolina A&T Aggies",
                  "North Carolina Asheville Bulldogs",
                  "North Carolina Central Eagles",
                  "North Carolina Charlotte 49ers",
                  "North Carolina Courage",
                  "North Carolina Greensboro Spartans",
                  "North Carolina State Wolfpack",
                  "North Carolina Tar Heels",
                  "North Carolina Wilmington Seahawks",
                  "North Dakota",
                  "North Dakota Fighting Hawks",
                  "North Dakota Fighting Sioux",
                  "North Dakota State Bison",
                  "North Eastern Warriors",
                  "North Florida Ospreys",
                  "North Korea",
                  "North Texas Mean Green",
                  "Northeast United FC",
                  "Northeastern Huskies",
                  "Northeastern Illinois Golden Eagles",
                  "Northern Arizona Lumberjacks",
                  "Northern Colorado Bears",
                  "Northern Illinois Huskies",
                  "Northern Iowa Panthers",
                  "Northern Kentucky Norse",
                  "Northwest Arkansas Naturals",
                  "Northwestern State Demons",
                  "Northwestern Wildcats",
                  "Norway",
                  "Norwich City",
                  "Notre Dame Fighting Irish",
                  "Nottingham Forest",
                  "Nurnberg",
                  "NYIT Bears",
                  "NYU Bobcats",
                  "NYU Violets",
                  "Nîmes Olympique",
                  "Oakland Athletics",
                  "Oakland Golden Grizzlies",
                  "Oakland Raiders",
                  "Odisha FC",
                  "Ogden Raptors",
                  "Ohio Bobcats",
                  "Ohio State Buckeyes",
                  "Oita Trinita",
                  "Oklahoma City RedHawks",
                  "Oklahoma City Thunder",
                  "Oklahoma Sooners",
                  "Oklahoma State Cowboys",
                  "Old Dominion Monarchs",
                  "Ole Miss Rebels",
                  "Oleksiy Oliynyk",
                  "Olympiacos Basketball",
                  "Omaha Mavericks",
                  "Omaha Royals",
                  "Oman",
                  "Omiya Ardija",
                  "Oral Roberts Golden Eagles",
                  "Oregon Ducks",
                  "Oregon State Beavers",
                  "Orem Owlz",
                  "Orix Buffaloes",
                  "Orlando City SC",
                  "Orlando Magic",
                  "Orlando Pride",
                  "OSAKA EVESSA",
                  "Osasuna",
                  "OTSUKA CORPORATION ALPHAS",
                  "Ottawa Redblacks",
                  "Ottawa Senators",
                  "Ovince Saint Preux",
                  "Pacific Boxers",
                  "Pacific FC",
                  "Pacific Tigers",
                  "Pakistan",
                  "Palau",
                  "Palermo",
                  "Palestine",
                  "Palm Beach Cardinals",
                  "Panama",
                  "Panathinaikos Basketball",
                  "Papua New Guinea",
                  "Paraguay",
                  "Parma",
                  "Parma Calcio",
                  "Patna Pirates",
                  "Patrick Thistle",
                  "Paul Felder",
                  "Paul Menard",
                  "Paulo Costa",
                  "Pawtucket Red Sox",
                  "Paços de Ferreira",
                  "Pedro Munhoz",
                  "Penn Quakers",
                  "Penn State Nittany Lions",
                  "Pennsylvania Quakers",
                  "Peoria Chiefs",
                  "Pepperdine Waves",
                  "Peru",
                  "Perugia",
                  "PGA",
                  "Philadelphia 76ers",
                  "Philadelphia Athletics",
                  "Philadelphia Eagles",
                  "Philadelphia Flyers",
                  "Philadelphia Phillies",
                  "Philadelphia Quakers",
                  "Philadelphia Union",
                  "Philadelphia Wings",
                  "Philippines",
                  "Phoenix Mercury",
                  "Phoenix Suns",
                  "Piacenza",
                  "Pisa",
                  "Pittsburgh Panthers",
                  "Pittsburgh Penguins",
                  "Pittsburgh Pirates",
                  "Pittsburgh Steelers",
                  "Plymouth Argyle",
                  "Poland",
                  "Portimonense SC",
                  "Portland Beavers",
                  "Portland Fire",
                  "Portland Pilots",
                  "Portland Sea Dogs",
                  "Portland State Vikings",
                  "Portland Thorns FC",
                  "Portland Timbers",
                  "Portland Trail Blazers",
                  "Porto",
                  "Portugal",
                  "Potomac Nationals",
                  "Prairie View Panthers",
                  "Presbyterian Blue Hose",
                  "Preston North End",
                  "Princeton Rays",
                  "Princeton Tigers",
                  "Providence Friars",
                  "PSG",
                  "PSV Eindhoven",
                  "Puerto Rico",
                  "Pulaski Mariners",
                  "Pune 7 Aces",
                  "Puneri Paltan",
                  "Punjab FC",
                  "Purdue Boilermakers",
                  "Qatar",
                  "QPR",
                  "Quad Cities River Bandits",
                  "Querétaro",
                  "Quess East Bengal",
                  "Quinnipiac Bobcats",
                  "Racing Louisville FC",
                  "Racing Santander",
                  "Radford Highlanders",
                  "Rafael dos Anjos",
                  "Rajasthan Royals",
                  "Ranchi Rays",
                  "Rancho Cucamonga Quakes",
                  "Randa Markos",
                  "Rangers",
                  "Rani Yahya",
                  "Raphael Assunção",
                  "Raquel Pennington",
                  "Ray Borg",
                  "Rayo Vallecano",
                  "RB Leipzig",
                  "RBC Roosendaal",
                  "Reading",
                  "Reading Phillies",
                  "Real Kashmir FC",
                  "Real Madrid",
                  "Real Madrid Basketball",
                  "Real Oviedo",
                  "Real Salt Lake",
                  "Real Sociedad",
                  "Real Zaragoza",
                  "Recreativo Huelva",
                  "Red Bull Racing",
                  "Refugee Olympic Team",
                  "Reggina",
                  "Renato Moicano",
                  "Renault DP World",
                  "Rennes",
                  "Reno Aces",
                  "RENOFA Yamaguchi",
                  "Rhode Island Rams",
                  "Ricardo Lamas",
                  "Rice Owls",
                  "Richard Petty",
                  "Richmond Flying Squirrels",
                  "Richmond Spiders",
                  "Ricky Stenhouse Jr.",
                  "Rider Broncs",
                  "Rio Ave",
                  "Rising Pune Supergiants",
                  "RIZING ZEPHYR FUKUOKA",
                  "RKC Waalwijk",
                  "Roasso Kumamoto",
                  "Rob Font",
                  "Robbie Lawler",
                  "Robert Morris Colonials",
                  "Robert Whittaker",
                  "Rochester Knighthawks",
                  "Rochester Red Wings",
                  "Rochester Royals",
                  "Roda JC Kerkrade",
                  "Roma",
                  "Romania",
                  "Rome Braves",
                  "Rose Namajunas",
                  "Ross County",
                  "Rotherham United",
                  "Round Rock Express",
                  "Roxanne Modafferi",
                  "Royal Challengers Bangalore",
                  "Russia",
                  "Rutgers Scarlet Knights",
                  "Rwanda",
                  "Ryan Blaney",
                  "Ryan Newman",
                  "RYUKYU GOLDEN KINGS",
                  "Sacramento Kings",
                  "Sacramento Monarchs",
                  "Sacramento River Cats",
                  "Sacred Heart Pioneers",
                  "Sagan Tosu",
                  "Saint Kitts and Nevis",
                  "Saint Lucia",
                  "Saint Mary's Gaels",
                  "Saint Vincent and the Grenadines",
                  "SAITAMA BRONCOS",
                  "Saitama Seibu Lions",
                  "Salem Red Sox",
                  "Salem-Keizer Volcanoes",
                  "Salt Lake Bees",
                  "Sam Houston State Bearkats",
                  "Samford Bulldogs",
                  "Samoa",
                  "Sampdoria",
                  "San Antonio Missions",
                  "San Antonio Silver Stars",
                  "San Antonio Spurs",
                  "San Diego Chargers",
                  "San Diego Clippers",
                  "San Diego Padres",
                  "San Diego Rockets",
                  "San Diego Seals",
                  "San Diego State Aztecs",
                  "San Diego Toreros",
                  "San Diego Wave FC",
                  "San Francisco 49ers",
                  "San Francisco Dons",
                  "San Francisco Giants",
                  "San Francisco Warriors",
                  "San Jose Earthquakes",
                  "San Jose Giants",
                  "San Jose Sharks",
                  "San Jose State Spartans",
                  "San Marino",
                  "SAN-EN NEOPHOENIX",
                  "Sanfrecce Hiroshima",
                  "Santa Clara Broncos",
                  "Santiago Ponzinibbio",
                  "Sao Paulo FC",
                  "Sara McMann",
                  "Saskatchewan Roughriders",
                  "Saskatchewan Rush",
                  "Sassuolo",
                  "Saudi Arabia",
                  "Savannah Sand Gnats",
                  "Savannah State Tigers",
                  "SC Cambuur",
                  "SC Sagamihara",
                  "Schalke",
                  "Scotland",
                  "Scranton/Wilkes-Barre Yankees",
                  "Scuderia AlphaTauri",
                  "Scuderia Ferrari",
                  "SD Eibar",
                  "SD Huesca",
                  "SD Ponferradina",
                  "SEAHORSES MIKAWA",
                  "Seattle Kraken",
                  "Seattle Mariners",
                  "Seattle Redhawks",
                  "Seattle Reign FC",
                  "Seattle Seahawks",
                  "Seattle Sounders FC",
                  "Seattle Storm",
                  "Seattle SuperSonics",
                  "Sedan",
                  "SENDAI EIGHTY NINERS",
                  "Senegal",
                  "Serbia",
                  "Serbia and Montenegro",
                  "Sergio Pettis",
                  "Seton Hall Pirates",
                  "Seychelles",
                  "Shamil Abdurakhimov",
                  "Sheffield United",
                  "Sheffield Wednesday",
                  "SHIGA LAKESTARS",
                  "SHIMANE SUSANOO MAGIC",
                  "Shimizu S-Pulse",
                  "SHINSHU BRAVE WARRIORS",
                  "Shonan Bellmare",
                  "Siena Saints",
                  "Sierra Leone",
                  "Sijara Eubanks",
                  "Singapore",
                  "SIU Edwardsville Cougars",
                  "Sky Blue FC",
                  "Slovakia",
                  "Slovenia",
                  "SM Caen",
                  "SMU Mustangs",
                  "Sochaux",
                  "Solomon Islands",
                  "Somalia",
                  "South Africa",
                  "South Alabama Jaguars",
                  "South Bend Silver Hawks",
                  "South Carolina Fighting Gamecocks",
                  "South Carolina State Bulldogs",
                  "South Dakota Coyotes",
                  "South Dakota State Jackrabbits",
                  "South Florida Bulls",
                  "South Korea",
                  "South Sudan",
                  "Southampton",
                  "Southeast Missouri State Indians",
                  "Southeast Missouri State Redhawks",
                  "Southeastern Louisiana Lions",
                  "Southern Illinois Salukis",
                  "Southern Jaguars",
                  "Southern Mississippi Golden Eagles",
                  "Southern Utah Thunderbirds",
                  "Southwest Missouri State Bears",
                  "Spain",
                  "Spal",
                  "Sparta Rotterdam",
                  "Spokane Indians",
                  "Sport Club Corinthians Paulista",
                  "Sport-Club Freiburg",
                  "Sporting",
                  "Sporting de Braga",
                  "Sporting Gijón",
                  "Sporting Kansas City",
                  "Springfield Cardinals",
                  "Sri Lanka",
                  "SSC Napoli",
                  "St Johnstone",
                  "St Mirren",
                  "St. Bonaventure Bonnies",
                  "St. Francis (New York) Terriers",
                  "St. Francis (Pennsylvania) Red Flash",
                  "St. Francis Brooklyn Terriers",
                  "St. John's Red Storm",
                  "St. Joseph's Hawks",
                  "St. Louis Blues",
                  "St. Louis Bombers",
                  "St. Louis Cardinals",
                  "St. Louis City",
                  "St. Louis Eagles",
                  "St. Louis Hawks",
                  "St. Louis Rams",
                  "St. Louis University Billikens",
                  "St. Lucie Mets",
                  "St. Mary's Rattlers",
                  "St. Peter's Peacocks",
                  "Stade de Reims",
                  "Stanford Cardinal",
                  "State College Spikes",
                  "Staten Island Yankees",
                  "Stefan Struve",
                  "Stephen F. Austin Lumberjacks",
                  "Stephen Thompson",
                  "Stetson Hatters",
                  "Stipe Miocic",
                  "Stockton Ports",
                  "Stoke City",
                  "Stony Brook Seawolves",
                  "Strasbourg",
                  "Sudan",
                  "Sunderland",
                  "Sunrisers Hyderabad",
                  "SUNROCKERS SHIBUYA",
                  "Suriname",
                  "Swansea City",
                  "Swaziland",
                  "Sweden",
                  "Switzerland",
                  "Syracuse Chiefs",
                  "Syracuse Nationals",
                  "Syracuse Orange",
                  "Syria",
                  "São Tomé and Príncipe",
                  "Tacoma Rainiers",
                  "Tai Tuivasa",
                  "Tajikistan",
                  "Tamil Thalaivas",
                  "Tampa Bay Buccaneers",
                  "Tampa Bay Lightning",
                  "Tampa Bay Rays",
                  "Tampa Rays",
                  "Tampa Yankees",
                  "Tanzania",
                  "Tatiana Suarez",
                  "TCU Horned Frogs",
                  "Team Cuba",
                  "Team Dominican Republic",
                  "Team Japan",
                  "Team Netherlands",
                  "Team Panama",
                  "Team Puerto Rico",
                  "Team South Korea",
                  "Team United States",
                  "Team Venezuela",
                  "Tecia Torres",
                  "Telugu Titans",
                  "Temple Owls",
                  "Tennessee Chattanooga Mocs",
                  "Tennessee Martin Skyhawks",
                  "Tennessee Smokies",
                  "Tennessee State Tigers",
                  "Tennessee Tech Golden Eagles",
                  "Tennessee Titans",
                  "Tennessee Volunteers",
                  "Tennis",
                  "Ternana",
                  "Texas A&M Aggies",
                  "Texas A&M-Corpus Christi Islanders",
                  "Texas Arlington Mavericks",
                  "Texas El Paso Miners",
                  "Texas Longhorns",
                  "Texas Pan American Broncs",
                  "Texas Rangers",
                  "Texas San Antonio Roadrunners",
                  "Texas Southern Tigers",
                  "Texas State Bobcats",
                  "Texas Tech Red Raiders",
                  "Texas-Rio Grande Valley Vaqueros",
                  "Thailand",
                  "The Gambia",
                  "Thespakusatsu Gunma",
                  "Thiago Santos",
                  "Thomas Almeida",
                  "Thonon Evian FC",
                  "Tiddim Road Athletic Union",
                  "Tim Elliott",
                  "TJ Dillashaw",
                  "TOCHIGI BREX",
                  "Tochigi SC",
                  "Togo",
                  "Tohoku Rakuten Golden Eagles",
                  "TOKIO MARINE NICHIDO BIG BLUE",
                  "Tokushima Vortis",
                  "TOKYO CINQ REVES",
                  "TOKYO EXCELLENCE",
                  "TOKYO HACHIOJI TRAINS",
                  "Tokyo Verdy1969",
                  "Tokyo Yakult Swallows",
                  "Toledo Mud Hens",
                  "Toledo Rockets",
                  "Tondela",
                  "Tonga",
                  "Tony Ferguson",
                  "Tony Stewart",
                  "Tonya Evinger",
                  "Torino",
                  "Toronto Arenas",
                  "Toronto Argonauts",
                  "Toronto Blue Jays",
                  "Toronto FC",
                  "Toronto Maple Leafs",
                  "Toronto Raptors",
                  "Toronto Rock",
                  "Toronto St. Pats",
                  "Toronto Tempo",
                  "Tottenham Hotspur",
                  "Toulouse FC",
                  "Towson Tigers",
                  "TOYAMA GROUSES",
                  "TOYODA GOSEI SCORPIONS",
                  "Trenton Thunder",
                  "Trevor Bayne",
                  "Tri-City Dust Devils",
                  "Tri-City ValleyCats",
                  "Trinidad and Tobago",
                  "Troy State Trojans",
                  "Troyes",
                  "TSG 1899 Hoffenheim",
                  "TSV 1860 Munich",
                  "Tulane Green Wave",
                  "Tulsa Drillers",
                  "Tulsa Golden Hurricane",
                  "Tulsa Shock",
                  "Tunisia",
                  "Turkey",
                  "Turkmenistan",
                  "Tuvalu",
                  "Twente Enschede",
                  "Ty Dillon",
                  "Tyron Woodley",
                  "Tyson Pedro",
                  "U Mumba",
                  "U Mumba Volley",
                  "UANL Tigres",
                  "UC Davis Aggies",
                  "UCLA Bruins",
                  "UD Almería",
                  "UD Las Palmas",
                  "Udinese",
                  "Uganda",
                  "Ukraine",
                  "Ulka Sasaki",
                  "UMass Lowell River Hawks",
                  "Union Berlin",
                  "United Arab Emirates",
                  "United States",
                  "UNLV Rebels",
                  "UP Dangal",
                  "UP Yoddha",
                  "Urawa Red Diamonds",
                  "Uriah Hall",
                  "Uruguay",
                  "US Salernitana",
                  "USC Trojans",
                  "USC Upstate Spartans",
                  "Utah Jazz",
                  "Utah Mammoth",
                  "Utah Royals FC",
                  "Utah State Aggies",
                  "Utah Utes",
                  "Utah Valley Wolverines",
                  "Uttar Pradesh Wizards",
                  "Uzbekistan",
                  "V-Varen Nagasaki",
                  "Valencia",
                  "Valencia Basketball",
                  "Valenciennes FC",
                  "Valentina Shevchenko",
                  "Valladolid",
                  "Valour FC",
                  "Valparaiso Crusaders",
                  "Vancouver Canadians",
                  "Vancouver Canucks",
                  "Vancouver FC",
                  "Vancouver Warriors",
                  "Vancouver Whitecaps",
                  "Vanderbilt Commodores",
                  "Vanuatu",
                  "Vegalta Sendai",
                  "Vegas Golden Knights",
                  "Venezia FC",
                  "Venezuela",
                  "Ventforet Kofu",
                  "Vermont Catamounts",
                  "Vermont Lake Monsters",
                  "Verona FC",
                  "VfB Stuttgart",
                  "VfL Bochum",
                  "VfL Osnabrück",
                  "VfL Wolfsburg",
                  "Vietnam",
                  "Villanova Wildcats",
                  "Villareal",
                  "Virgin Islands",
                  "Virginia Cavaliers",
                  "Virginia Commonwealth Rams",
                  "Virginia Tech Hokies",
                  "Visalia Rawhide",
                  "Vissel Kobe",
                  "Vitesse Arnhem",
                  "Vitória Guimarães",
                  "Vitória Setúbal",
                  "VMI Keydets",
                  "Volkan Oezdemir",
                  "Wagner Seahawks",
                  "Wake Forest Demon Deacons",
                  "Wales",
                  "Washington Capitals",
                  "Washington Commanders",
                  "Washington Football Team",
                  "Washington Huskies",
                  "Washington Mystics",
                  "Washington Nationals",
                  "Washington Spirit",
                  "Washington State Cougars",
                  "Washington Wizards",
                  "Watford",
                  "Weber State Wildcats",
                  "Werder Bremen",
                  "West Bromwich Albion",
                  "West Ham United",
                  "West Indies",
                  "West Michigan Whitecaps",
                  "West Tenn Diamond Jaxx",
                  "West Virginia Mountaineers",
                  "West Virginia Power",
                  "Western Carolina Catamounts",
                  "Western Illinois Leathernecks",
                  "Western Kentucky Hilltoppers",
                  "Western Michigan Broncos",
                  "Wichita State Shockers",
                  "Wigan",
                  "Willem II Tilburg",
                  "William & Mary Tribe",
                  "William Byron",
                  "Williams Racing",
                  "Williamsport Crosscutters",
                  "Wilmington Blue Rocks",
                  "Wilson Reis",
                  "Winnipeg Blue Bombers",
                  "Winnipeg Jets",
                  "Winston-Salem Dash",
                  "Winthrop Eagles",
                  "Wisconsin Badgers",
                  "Wisconsin Green Bay Phoenix",
                  "Wisconsin Milwaukee Panthers",
                  "Wisconsin Timber Rattlers",
                  "Wofford Terriers",
                  "Wolverhampton Wanderers",
                  "Wright State Raiders",
                  "WUSA",
                  "WWE",
                  "Wyoming Cowboys",
                  "X-Games",
                  "Xavier Musketeers",
                  "Yair Rodriguez",
                  "Yakima Bears",
                  "Yale Bulldogs",
                  "YAMAGATA WYVERNS",
                  "Yana Kunitskaya",
                  "Yemen",
                  "Yoel Romero",
                  "YOKOHAMA B-CORSAIRS",
                  "Yokohama DeNA BayStars",
                  "Yokohama F. Marinos",
                  "Yokohama FC",
                  "Yomiuri Giants",
                  "York United FC",
                  "Youngstown State Penguins",
                  "YSCC Yokohama",
                  "Yugoslavia",
                  "Zabit Magomedsharipov",
                  "Zalgiris Kaunas Basketball",
                  "Zambia",
                  "Zenit St Petersburg Basketball",
                  "Zimbabwe",
                  "Zweigen Kanazawa"
                ],
                "type": "string",
                "enumNames": [
                  "1. FC Koln",
                  "1. FC Magdeburg",
                  "A. J. Allmendinger",
                  "A.S. Livorno Calcio",
                  "Aberdeen",
                  "Aberdeen IronBirds",
                  "Abilene Christian Wildcats",
                  "AC Ajaccio",
                  "AC Milan",
                  "AC Nagano Parceiro",
                  "AD Alcorcón",
                  "ADO Den Haag",
                  "AFC Bournemouth",
                  "Afghanistan",
                  "Ahmedabad Defenders",
                  "Air Force Falcons",
                  "Airdrieonians",
                  "AISIN AW AREIONS ANJO",
                  "Aizawl FC",
                  "Ajax Amsterdam",
                  "AKITA NORTHERN HAPPINETS",
                  "Akron Aeros",
                  "Akron Zips",
                  "Al Iaquinta",
                  "Alabama A&M Bulldogs",
                  "Alabama Birmingham Blazers",
                  "Alabama Crimson Tide",
                  "Alabama State Hornets",
                  "Alaves",
                  "ALBA Berlin Basketball",
                  "Albacete BP",
                  "Albania",
                  "Albany Great Danes",
                  "Albirex Niigata",
                  "Albuquerque Isotopes",
                  "Alcorn State Braves",
                  "Alejandro Perez",
                  "Alex Bowman",
                  "Alex Oliveira",
                  "Alex Perez",
                  "Alexa Grasso",
                  "Alexander Gustafsson",
                  "Alexander Hernandez",
                  "Alexander Volkanoski",
                  "Alexander Volkov",
                  "Alexandre Pantoja",
                  "Alexis Davis",
                  "Alfa Romeo Racing",
                  "Algeria",
                  "Alistair Overeem",
                  "Aljamain Sterling",
                  "Almere City",
                  "Alpine",
                  "Altoona Curve",
                  "ALVARK TOKYO",
                  "Amanda Nunes",
                  "American Samoa",
                  "American University Eagles",
                  "Amiens SC",
                  "Anadolu Efes Istanbul Basketball",
                  "Anaheim Ducks",
                  "Andorra",
                  "Andrea Lee",
                  "Andrei Arlovski",
                  "Angel City FC",
                  "Angela Hill",
                  "Angers SCO",
                  "Angola",
                  "Anthony Pettis",
                  "Anthony Smith",
                  "Antigua and Barbuda",
                  "Antonio Carlos Junior",
                  "AOMORI WAT'S",
                  "Appalachian State Mountaineers",
                  "Arbroath",
                  "Argentina",
                  "Aric Almirola",
                  "Arizona Cardinals",
                  "Arizona Coyotes",
                  "Arizona Diamondbacks",
                  "Arizona State Sun Devils",
                  "Arizona Wildcats",
                  "Arkansas Little Rock Trojans",
                  "Arkansas Razorbacks",
                  "Arkansas State Indians",
                  "Arkansas State Red Wolves",
                  "Arkansas Travelers",
                  "Arkansas-Pine Bluff Golden Lions",
                  "Armenia",
                  "Arminia Bielefeld",
                  "Army Black Knights",
                  "Arsenal",
                  "Arsenal de Sarandí",
                  "Aruba",
                  "AS Roma",
                  "AS Saint-Etienne",
                  "Ascoli",
                  "Asheville Tourists",
                  "Ashlee Evans-Smith",
                  "Aspen Ladd",
                  "Aston Martin",
                  "Aston Villa",
                  "Atalanta",
                  "Athletic Bilbao",
                  "ATK Mohun Bagan FC",
                  "Atlanta Braves",
                  "Atlanta Dream",
                  "Atlanta Falcons",
                  "Atlanta Flames",
                  "Atlanta Hawks",
                  "Atlanta Thrashers",
                  "Atlanta United FC",
                  "Atletico Madrid",
                  "Atlético de San Luis",
                  "Atlético Ottawa",
                  "Auburn Doubledays",
                  "Auburn Tigers",
                  "Augusta GreenJackets",
                  "Austin Dillon",
                  "Austin FC",
                  "Austin Peay Governors",
                  "Australia",
                  "Austria",
                  "Auxerre",
                  "Avispa Fukuoka",
                  "Awadhe Warriors",
                  "AX Armani Exchange Milan Basketball",
                  "AZ Alkmaar",
                  "Azerbaijan",
                  "Bahamas",
                  "Bahrain",
                  "Bakersfield Blaze",
                  "Ball State Cardinals",
                  "Baltimore Orioles",
                  "Baltimore Ravens",
                  "BAMBITIOUS NARA",
                  "Bangladesh",
                  "Barbados",
                  "Barcelona",
                  "Barcelona Basketball",
                  "Bari",
                  "Bastia",
                  "Batavia Muckdogs",
                  "Bates Bobcats",
                  "Bayer Leverkusen",
                  "Bayern Munich",
                  "Bayern Munich Basketball",
                  "Baylor Bears",
                  "BC Lions",
                  "Belarus",
                  "Belenenses",
                  "Belgium",
                  "Belize",
                  "Belmont Bruins",
                  "Beloit Snappers",
                  "Ben Nguyen",
                  "Benfica",
                  "Bengal Warriors",
                  "Bengaluru Bulls",
                  "Bengaluru FC",
                  "Bengaluru Raptors",
                  "Benin",
                  "Bermuda",
                  "Bethe Correia",
                  "Bethune Cookman Wildcats",
                  "Betis Sevilla",
                  "Bhutan",
                  "Billings Mustangs",
                  "Binghamton Bearcats",
                  "Binghamton Mets",
                  "Birmingham Barons",
                  "Birmingham City",
                  "Black Hawks Hyderabad",
                  "Blackburn Rovers",
                  "Blaublitz Akita",
                  "Bluefield Orioles",
                  "Boavista",
                  "Bobby Labonte",
                  "Boca Juniors",
                  "Boise Hawks",
                  "Boise State Broncos",
                  "Bolivia",
                  "Bologna",
                  "Bolton Wanderers",
                  "Bordeaux",
                  "Borussia Dortmund",
                  "Borussia Monchengladbach",
                  "Bosnia and Herzegovina",
                  "Boston Beaneaters",
                  "Boston Beans",
                  "Boston Bruins",
                  "Boston Celtics",
                  "Boston College Eagles",
                  "Boston Legacy FC",
                  "Boston Patriots",
                  "Boston Red Sox",
                  "Boston Redskins",
                  "Boston University Terriers",
                  "Botswana",
                  "Bowie Baysox",
                  "Bowling Green Falcons",
                  "Bowling Green Hot Rods",
                  "Brad Keselowski",
                  "Brad Tavares",
                  "Bradenton Marauders",
                  "Bradley Braves",
                  "Brandon Moreno",
                  "Brazil",
                  "Brentford",
                  "Brescia",
                  "Brest",
                  "Brevard County Manatees",
                  "Brian Ortega",
                  "Brighton & Hove Albion",
                  "Bristol City",
                  "Bristol White Sox",
                  "British Virgin Islands",
                  "Brooklyn Cyclones",
                  "Brooklyn Nets",
                  "Brown Bears",
                  "Brunei",
                  "Bryant Bulldogs",
                  "Bucknell Bison",
                  "Buffalo Bandits",
                  "Buffalo Bills",
                  "Buffalo Bisons",
                  "Buffalo Braves",
                  "Buffalo Bulls",
                  "Buffalo Sabres",
                  "Bulgaria",
                  "Burkina Faso",
                  "Burlington Bees",
                  "Burlington Royals",
                  "Burnley",
                  "Burundi",
                  "Butler Bulldogs",
                  "BWT Racing Point",
                  "BYU Cougars",
                  "C.D. Chivas USA",
                  "CA River Plate",
                  "Cagliari Calcio",
                  "Cal Irvine Anteaters",
                  "Cal Poly Mustangs",
                  "Cal Riverside Highlanders",
                  "Cal Santa Barbara Gauchos",
                  "Cal State Bakersfield Roadrunners",
                  "Cal State Fullerton Titans",
                  "Cal State Northridge Matadors",
                  "Cal State Sacramento Hornets",
                  "Calcio Catania",
                  "Calgary Flames",
                  "Calgary Roughnecks",
                  "Calgary Stampeders",
                  "Calicut Heroes",
                  "California Angels",
                  "California Baptist Lancers",
                  "California Golden Bears",
                  "California Seals",
                  "Cambodia",
                  "Cameroon",
                  "Campbell Fighting Camels",
                  "Canada",
                  "Canisius Golden Griffins",
                  "Cape Verde",
                  "Cardiff City",
                  "Carl Edwards",
                  "Carla Esparza",
                  "Carolina Hurricanes",
                  "Carolina Mudcats",
                  "Carolina Panthers",
                  "Casa Pia AC",
                  "Casey Mears",
                  "Casper Ghosts",
                  "Cat Zingano",
                  "Catanzaro",
                  "Cavalry FC",
                  "Cayman Islands",
                  "CD Lugo",
                  "CD Mirandés",
                  "CD Numancia",
                  "CD Santa Clara",
                  "CD Tenerife",
                  "Cedar Rapids Kernels",
                  "Celta Vigo",
                  "Celtic",
                  "Centenary Gentlemen",
                  "Central African Republic",
                  "Central Arkansas Bears",
                  "Central Connecticut Blue Devils",
                  "Central Connecticut State Blue Devils",
                  "Central Florida Golden Knights",
                  "Central Michigan Chippewas",
                  "Cerezo Osaka",
                  "CF Atlas",
                  "CF Estrela",
                  "CF Fuenlabrada",
                  "CF Monterrey",
                  "Chad",
                  "Chad Mendes",
                  "Chan Sung Jung",
                  "Charleston Cougars",
                  "Charleston RiverDogs",
                  "Charleston Southern Buccaneers",
                  "Charlotte 49ers",
                  "Charlotte Hornets",
                  "Charlotte Knights",
                  "Charlotte Sting",
                  "Charlotte Stone Crabs",
                  "Charlton Athletic",
                  "Chase Elliott",
                  "Chattanooga Lookouts",
                  "Chaves",
                  "Chelsea",
                  "Chennai City FC",
                  "Chennai Spartans",
                  "Chennai Super Kings",
                  "Chennai Superstarz",
                  "Chennaiyin FC",
                  "CHIBA JETS",
                  "Chiba Lotte Marines",
                  "Chicago Bears",
                  "Chicago Blackhawks",
                  "Chicago Bulls",
                  "Chicago Cardinals",
                  "Chicago Cubs",
                  "Chicago Fire",
                  "Chicago Red Stars",
                  "Chicago Sky",
                  "Chicago Stags",
                  "Chicago State Cougars",
                  "Chicago White Sox",
                  "Chicago White Stockings",
                  "Chicago Whitesox",
                  "Chicago Zephyrs",
                  "Chievo Verona",
                  "Chile",
                  "China",
                  "Chinese Taipei",
                  "Chris Buescher",
                  "Chris Weidman",
                  "Chunichi Dragons",
                  "Churchill Brothers FC Goa",
                  "Cincinnati Bearcats",
                  "Cincinnati Bengals",
                  "Cincinnati Redlegs",
                  "Cincinnati Reds",
                  "Citadel Bulldogs",
                  "Cittadella",
                  "Claudia Gadelha",
                  "Clearwater Threshers",
                  "Clemson Tigers",
                  "Clermont Foot 63",
                  "Cleveland Barons",
                  "Cleveland Blues",
                  "Cleveland Browns",
                  "Cleveland Cavaliers",
                  "Cleveland Indians",
                  "Cleveland Naps",
                  "Cleveland Rockers",
                  "Cleveland State Vikings",
                  "Clint Bowyer",
                  "Clinton LumberKings",
                  "Club América",
                  "Club Atlético River Plate",
                  "Club Deportivo Guadalajara - Chivas",
                  "Club Deportivo Social y Cultural - Cruz Azul",
                  "Club Santos Laguna",
                  "Club Universidad Nacional A.C. - Pumas",
                  "Coastal Carolina Chanticleers",
                  "Cody Garbrandt",
                  "Cody Stamann",
                  "Colby Covington",
                  "Colgate Raiders",
                  "Colombia",
                  "Colorado Avalanche",
                  "Colorado Buffaloes",
                  "Colorado College Tigers",
                  "Colorado Mammoth",
                  "Colorado Rapids",
                  "Colorado Rockies",
                  "Colorado Springs Sky Sox",
                  "Colorado State Rams",
                  "Columbia Lions",
                  "Columbus Blue Jackets",
                  "Columbus Clippers",
                  "Columbus Crew",
                  "Como",
                  "Comoros",
                  "Congo",
                  "Connecticut Huskies",
                  "Connecticut Sun",
                  "Connecticut Tigers",
                  "Conor McGregor",
                  "Consadole Sapporo",
                  "Cook Islands",
                  "Coppin State Eagles",
                  "Corey Anderson",
                  "Cornell Big Red",
                  "Corpus Christi Hooks",
                  "Cortney Casey",
                  "Cosenza",
                  "Costa Rica",
                  "Cote d'Ivoire",
                  "Coventry City",
                  "Creighton Bluejays",
                  "Cris Cyborg",
                  "Croatia",
                  "Crvena Zvezda mts Belgrade Basketball",
                  "Crystal Palace",
                  "CSKA Moscow Basketball",
                  "Cub Swanson",
                  "Cuba",
                  "Curtis Blaydes",
                  "Cyprus",
                  "Czech Republic",
                  "Cádiz CF",
                  "D.C. United",
                  "Dabang Delhi KC",
                  "Dabang Mumbai HC",
                  "Dale Earnhardt",
                  "Dale Earnhardt Jr.",
                  "Dallas Baptist Patriots",
                  "Dallas Cowboys",
                  "Dallas Mavericks",
                  "Dallas Stars",
                  "Dallas Texans",
                  "Dallas Wings",
                  "Dan Hooker",
                  "Daniel Cormier",
                  "Daniel Suárez",
                  "Danville Braves",
                  "Darmstadt 98",
                  "Darrell Wallace Jr.",
                  "Darren Elkins",
                  "Darren Till",
                  "Dartmouth Big Green",
                  "David Branch",
                  "David Ragan",
                  "Davidson Wildcats",
                  "Dayton Dragons",
                  "Dayton Flyers",
                  "Daytona Cubs",
                  "De Graafschap",
                  "Deiveson Figueiredo",
                  "Delaware Fightin' Blue Hens",
                  "Delaware State Hornets",
                  "Delhi Capitals",
                  "Delhi Sultans",
                  "Delhi Waveriders",
                  "Delmarva Shorebirds",
                  "Demian Maia",
                  "Democratic Republic of the Congo",
                  "Denmark",
                  "Denny Hamlin",
                  "Denver Broncos",
                  "Denver Nuggets",
                  "Denver Pioneers",
                  "DePaul Blue Demons",
                  "Deportivo La Coruna",
                  "Derby County",
                  "Derek Brunson",
                  "Derrick Lewis",
                  "Desportivo das Aves",
                  "Detroit Cougars",
                  "Detroit Falcons",
                  "Detroit Lions",
                  "Detroit Pistons",
                  "Detroit Red Wings",
                  "Detroit Shock",
                  "Detroit Tigers",
                  "Detroit Titans",
                  "Dijon FCO",
                  "Djibouti",
                  "Dominica",
                  "Dominican Republic",
                  "Dominick Cruz",
                  "Dominick Reyes",
                  "Donald Cerrone",
                  "Douglas Silva de Andrade",
                  "Drake Bulldogs",
                  "Drexel Dragons",
                  "Duke Blue Devils",
                  "Dundee",
                  "Dundee United",
                  "Dunedin Blue Jays",
                  "Dunfermline",
                  "Duquesne Dukes",
                  "Durham Bulls",
                  "Dustin Ortiz",
                  "Dustin Poirier",
                  "Dynamo Dresden",
                  "E-Sports",
                  "EARTHFRIENDS TOKYO Z",
                  "East Carolina Pirates",
                  "East Tennessee State Buccaneers",
                  "East Timor",
                  "Eastern Illinois Panthers",
                  "Eastern Kentucky Colonels",
                  "Eastern Michigan Eagles",
                  "Eastern Washington Eagles",
                  "Ecuador",
                  "Edmonton Football Team",
                  "Edmonton Oilers",
                  "Edson Barboza",
                  "Egypt",
                  "Ehime FC",
                  "EHIME ORANGE VIKINGS",
                  "Eintracht Braunschweig",
                  "Eintracht Frankfurt",
                  "El Salvador",
                  "Elche CF",
                  "Elias Theodorou",
                  "Elizabethton Twins",
                  "Elizeu Zaleski dos Santos",
                  "Elliott Sadler",
                  "Elon Phoenix",
                  "Empoli",
                  "Energie Cottbus",
                  "England",
                  "Equatorial Guinea",
                  "Erie SeaWolves",
                  "Erik Jones",
                  "Eritrea",
                  "Espanyol",
                  "Estonia",
                  "Estoril",
                  "Ethiopia",
                  "Eugene Emeralds",
                  "Evansville Purple Aces",
                  "Everett AquaSox",
                  "Everton",
                  "Excelsior",
                  "Extremadura UD",
                  "F EAGLES NAGOYA",
                  "F.C. Gifu",
                  "Fagiano Okayama FC",
                  "Fairfield Stags",
                  "Fairleigh Dickinson Devils",
                  "Fairleigh Dickinson Knights",
                  "Famalicão",
                  "Farense",
                  "FC Arouca",
                  "FC Arsenal Tula",
                  "FC Augsburg",
                  "FC Basel",
                  "FC Cincinnati",
                  "FC Dallas",
                  "FC Edmonton",
                  "FC Goa",
                  "FC Groningen",
                  "FC Heidenheim",
                  "FC Juárez",
                  "FC Lorient",
                  "FC Machida Zelvia",
                  "FC Ryūkyū",
                  "FC Sevilla",
                  "FC St. Pauli",
                  "FC Startak Moscow",
                  "FC Tokyo",
                  "FC Utrecht",
                  "FC Volendam",
                  "FC Zwolle",
                  "Federated States of Micronesia",
                  "Felice Herrig",
                  "Fenerbahce Beko Istanbul",
                  "Feyenoord Rotterdam",
                  "Fiji",
                  "Finland",
                  "Fiorentina",
                  "FIU Panthers",
                  "Florida A&M Rattlers",
                  "Florida Atlantic Owls",
                  "Florida Gators",
                  "Florida Gulf Coast Eagles",
                  "Florida International Golden Panthers",
                  "Florida Panthers",
                  "Florida State Seminoles",
                  "Fordham Rams",
                  "Forge FC",
                  "Fort Myers Miracle",
                  "Fort Wayne Mastodons",
                  "Fort Wayne Pistons",
                  "Fort Wayne TinCaps",
                  "Fortuna Düsseldorf",
                  "Fortuna Sittard",
                  "France",
                  "Francis Ngannou",
                  "Francisco Trinaldo",
                  "Frankie Edgar",
                  "Frederick Keys",
                  "Fresno Grizzlies",
                  "Fresno State Bulldogs",
                  "Frisco RoughRiders",
                  "Frosinone FC",
                  "FSV Mainz 05",
                  "Fujieda MYFC",
                  "Fukuoka SoftBank Hawks",
                  "FUKUSHIMA FIREBONDS",
                  "Fukushima United FC",
                  "Fulham",
                  "Furman Paladins",
                  "Gabon",
                  "Gainare Tottori",
                  "Galatasaray SK",
                  "Gamba Osaka",
                  "Gardner-Webb Runnin' Bulldogs",
                  "Genoa",
                  "George Mason Patriots",
                  "George Washington Colonials",
                  "Georges St-Pierre",
                  "Georgetown Hoyas",
                  "Georgia",
                  "Georgia Bulldogs",
                  "Georgia Southern Eagles",
                  "Georgia State Panthers",
                  "Georgia Swarm",
                  "Georgia Tech Yellow Jackets",
                  "Germaine de Randamie",
                  "Germany",
                  "Getafe CF",
                  "Getafe FC",
                  "Ghana",
                  "Gil Vicente",
                  "Giravanz Kitakyushu",
                  "Girona FC",
                  "Glover Teixeira",
                  "Go Ahead Eagles",
                  "Gokulam Kerala FC",
                  "Golden State Valkyries",
                  "Golden State Warriors",
                  "Gonzaga Bulldogs",
                  "Grambling Tigers",
                  "Granada CF",
                  "Grand Canyon Antelopes",
                  "Gray Gaulding",
                  "Great Britain",
                  "Great Falls Voyagers",
                  "Great Lakes Loons",
                  "Greece",
                  "Green Bay Packers",
                  "Greeneville Astros",
                  "Greensboro Grasshoppers",
                  "Greenville Drive",
                  "Greg Biffle",
                  "Grenada",
                  "Greuther Fürth",
                  "Grulla Morioka",
                  "Guam",
                  "Guatemala",
                  "Guinea",
                  "Guinea-Bissau",
                  "Guingamp",
                  "Gujarat Fortunegiants",
                  "Gujarat Lions",
                  "GUNMA CRANE THUNDERS",
                  "Gunnar Nelson",
                  "Guyana",
                  "Gwinnett Braves",
                  "Haas F1 Team",
                  "Hagerstown Suns",
                  "Haiti",
                  "Halifax Thunderbirds",
                  "Hamburg SV",
                  "Hamilton Tiger-Cats",
                  "Hamilton Tigers",
                  "Hampton Pirates",
                  "Hannover 96",
                  "Hansa Rostock",
                  "Hanshin Tigers",
                  "Harrisburg Senators",
                  "Hartford Hawks",
                  "Hartford Whalers",
                  "Harvard Crimson",
                  "Haryana Hammers",
                  "Haryana Steelers",
                  "Hawaii Rainbow Warriors",
                  "Hearts",
                  "Heerenveen",
                  "Helena Brewers",
                  "Henry Cejudo",
                  "Heracles Almelo",
                  "Hertha Berlin",
                  "Hertha BSC",
                  "HFX Wanderers FC",
                  "Hibernian",
                  "Hickory Crawdads",
                  "High Desert Mavericks",
                  "High Point Panthers",
                  "High School Baseball Team",
                  "HIROSHIMA DRAGONFLIES",
                  "Hiroshima Toyo Carp",
                  "Hofstra Flying Dutchmen",
                  "Hofstra Pride",
                  "Hokkaido Nippon-Ham Fighters",
                  "Holly Holm",
                  "Holy Cross Crusaders",
                  "Honduras",
                  "Hong Kong",
                  "Houston Astros",
                  "Houston Baptist Huskies",
                  "Houston Comets",
                  "Houston Cougars",
                  "Houston Dash",
                  "Houston Dynamo",
                  "Houston Oilers",
                  "Houston Rockets",
                  "Houston Texans",
                  "Howard Bison",
                  "Huddersfield Town",
                  "Hudson Valley Renegades",
                  "Hull City",
                  "Hungary",
                  "Huntsville Stars",
                  "Hyderabad FC",
                  "Hyderabad Hunters",
                  "IBARAKI ROBOTS",
                  "Iceland",
                  "Idaho Falls Chukars",
                  "Idaho State Bengals",
                  "Idaho Vandals",
                  "Ilir Latifi",
                  "Illinois Chicago Flames",
                  "Illinois Illini",
                  "Illinois State Redbirds",
                  "Incarnate Word Cardinals",
                  "Independent Olympic Athletes",
                  "India",
                  "Indian Arrows",
                  "Indiana Fever",
                  "Indiana Hoosiers",
                  "Indiana Pacers",
                  "Indiana State Sycamores",
                  "Indianapolis Colts",
                  "Indianapolis Indians",
                  "Indonesia",
                  "Inland Empire 66ers",
                  "Inter Miami CF",
                  "Inter Milan",
                  "Inverness Caledonian Thistle",
                  "Iona Gaels",
                  "Iowa Cubs",
                  "Iowa Hawkeyes",
                  "Iowa State Cyclones",
                  "IPFW Mastodons",
                  "Ipswich Town",
                  "Iran",
                  "Iraq",
                  "Ireland",
                  "Irene Aldana",
                  "Israel",
                  "Israel Adesanya",
                  "Italy",
                  "IUPUI Jaguars",
                  "Ivory Coast",
                  "Iwaki FC",
                  "IWATE BIG BULLS",
                  "Jacare Souza",
                  "Jackson State Tigers",
                  "Jacksonville Dolphins",
                  "Jacksonville Jaguars",
                  "Jacksonville State Gamecocks",
                  "Jacksonville Suns",
                  "Jaipur Pink Panthers",
                  "Jamaica",
                  "James Madison Dukes",
                  "James Vick",
                  "Jamestown Jammers",
                  "Jamie McMurray",
                  "Jamshedpur FC",
                  "Jan Blachowicz",
                  "Japan",
                  "Jared Cannonier",
                  "Jaypee Punjab Warriors",
                  "JEF United Ichihara Chiba",
                  "Jeff Burton",
                  "Jeff Gordon",
                  "Jennifer Maia",
                  "Jeremy Stephens",
                  "Jessica Andrade",
                  "Jessica Eye",
                  "Jessica-Rose Clark",
                  "Jimi Manuwa",
                  "Jimmie Johnson",
                  "Jimmie Rivera",
                  "Joanna Jedrzejczyk",
                  "Joanne Calderwood",
                  "Joey Logano",
                  "John Dodson",
                  "John Lineker",
                  "John Moraga",
                  "Johnson City Cardinals",
                  "Jon Jones",
                  "Jordan",
                  "Jorge Masvidal",
                  "Jose Aldo",
                  "Joseph Benavidez",
                  "Josh Emmett",
                  "Juan Pablo Montoya",
                  "Julianna Pena",
                  "Junior dos Santos",
                  "Jupiter Hammerheads",
                  "Jussier Formiga",
                  "Justin Gaethje",
                  "Justin Willis",
                  "Juventus",
                  "Júbilo Iwata",
                  "KAGAWA FIVE ARROWS",
                  "KAGOSHIMA REBNISE",
                  "Kaiserslautern",
                  "Kalinga Lancers",
                  "Kamaru Usman",
                  "Kamatamare Sanuki",
                  "KANAZAWA SAMURAIZ",
                  "Kane County Cougars",
                  "Kannapolis Intimidators",
                  "Kansas City Athletics",
                  "Kansas City Chiefs",
                  "Kansas City Current",
                  "Kansas City Kings",
                  "Kansas City Royals",
                  "Kansas City Scouts",
                  "Kansas Jayhawks",
                  "Kansas State Wildcats",
                  "Karlsruher SC",
                  "Karolina Kowalkiewicz",
                  "Kasey Kahne",
                  "Kashima Antlers",
                  "Kashiwa Reysol",
                  "Kataller Toyama",
                  "Katlyn Chookagian",
                  "KAWASAKI BRAVE THUNDERS",
                  "Kawasaki Frontale",
                  "Kazakhstan",
                  "Kelvin Gastelum",
                  "Kennesaw State Owls",
                  "Kent State Golden Flashes",
                  "Kentucky Wildcats",
                  "Kenya",
                  "Kerala Blasters FC",
                  "Ketlen Vieira",
                  "Kevin Harvick",
                  "Kevin Lee",
                  "Khabib Nurmagomedov",
                  "Khimki Moscow Region Basketball",
                  "Kilmarnock",
                  "Kings XI Punjab",
                  "Kingsport Mets",
                  "Kinston Indians",
                  "Kiribati",
                  "KIROLBET Baskonia Vitoria-Gasteiz Basketball",
                  "Kochi Blue Spikers",
                  "Kolkata Knight Riders",
                  "Kosovo",
                  "KUMAMOTO VOLTERS",
                  "Kurt Busch",
                  "Kyle Busch",
                  "Kyle Larson",
                  "KYOTO HANNARYZ",
                  "Kyoto Sanga FC",
                  "Kyrgyzstan",
                  "La Salle Explorers",
                  "Lafayette Leopards",
                  "Lake County Captains",
                  "Lake Elsinore Storm",
                  "Lakeland Flying Tigers",
                  "Lakewood BlueClaws",
                  "Lamar Cardinals",
                  "Lancaster JetHawks",
                  "Lansing Lugnuts",
                  "Laos",
                  "Las Vegas 51s",
                  "Las Vegas Aces",
                  "Las Vegas Raiders",
                  "Latvia",
                  "Lauren Murphy Increase1",
                  "Lazio",
                  "LDLC ASVEL Villeurbanne",
                  "Le Havre",
                  "Lebanon",
                  "Lecce",
                  "Lecco",
                  "Leeds United",
                  "Leganés",
                  "Lehigh Mountain Hawks",
                  "Lehigh Valley IronPigs",
                  "Leicester City",
                  "Lens",
                  "Leon Edwards",
                  "Lesotho",
                  "LEVANGA HOKKAIDO",
                  "Levante UD",
                  "Lexington Legends",
                  "Liberia",
                  "Liberty Flames",
                  "Libya",
                  "Liechtenstein",
                  "Lille",
                  "Lina Lansberg",
                  "Lipscomb Bisons",
                  "Lithuania",
                  "Liverpool",
                  "Livingston",
                  "Liz Carmouche",
                  "Long Beach State 49ers",
                  "Long Beach State Sharks",
                  "Long Island Blackbirds",
                  "Longwood Lancers",
                  "Los Angeles Angels",
                  "Los Angeles Chargers",
                  "Los Angeles Clippers",
                  "Los Angeles Dodgers",
                  "Los Angeles FC",
                  "Los Angeles Galaxy",
                  "Los Angeles Kings",
                  "Los Angeles Lakers",
                  "Los Angeles Rams",
                  "Los Angeles Sparks",
                  "Louisiana Lafayette Ragin' Cajuns",
                  "Louisiana Monroe Indians",
                  "Louisiana Tech Bulldogs",
                  "Louisiana-Monroe Warhawks",
                  "Louisville Bats",
                  "Louisville Cardinals",
                  "Lowell Spinners",
                  "Loyola Chicago Ramblers",
                  "Loyola Maryland Greyhounds",
                  "Loyola Marymount Lions",
                  "LPGA",
                  "LSU Tigers",
                  "Lucie Pudilova",
                  "Luke Rockhold",
                  "Luton Town",
                  "Luxembourg",
                  "Lynchburg Hillcats",
                  "Lyon",
                  "Maccabi FOX Tel Aviv Basketball",
                  "Macedonia",
                  "Mackenzie Dern",
                  "Madagascar",
                  "Mahoning Valley Scrappers",
                  "Maine Black Bears",
                  "Malaga",
                  "Malawi",
                  "Malaysia",
                  "Maldives",
                  "Mali",
                  "Mallorca",
                  "Malta",
                  "Manchester City",
                  "Manchester United",
                  "Manhattan Jaspers",
                  "Mara Romero Borella",
                  "Marcin Tybura",
                  "Marion Reneau",
                  "Marist Red Foxes",
                  "Mark Hunt",
                  "Mark Martin",
                  "Marlon Moraes",
                  "Marquette Golden Eagles",
                  "Marseille",
                  "Marshall Islands",
                  "Marshall Thundering Herd",
                  "Martin Truex Jr.",
                  "Maryland Baltimore County Retrievers",
                  "Maryland Eastern Shore Fighting Hawks",
                  "Maryland Terrapins",
                  "Marítimo",
                  "Massachusetts Minutemen",
                  "Matheus Nicolau",
                  "Matsumoto Yamaga FC",
                  "Matt DiBenedetto",
                  "Matt Kenseth",
                  "Mauricio Rua",
                  "Mauritania",
                  "Mauritius",
                  "Max Holloway",
                  "Mazatlán",
                  "Mclaren",
                  "McNeese State Cowboys",
                  "Memphis Grizzlies",
                  "Memphis Redbirds",
                  "Memphis Tigers",
                  "Mercedes-AMG Petronas",
                  "Mercer Bears",
                  "Metz",
                  "Mexico",
                  "Miami (Ohio) Redhawks",
                  "Miami Dolphins",
                  "Miami Heat",
                  "Miami Hurricanes",
                  "Miami Marlins",
                  "Miami Sol",
                  "Michael Chiesa",
                  "Michael McDowell",
                  "Michelle Waterson",
                  "Michigan State Spartans",
                  "Michigan Wolverines",
                  "Middle Tennessee State Blue Raiders",
                  "Middlesbrough",
                  "Middleweight",
                  "Midland RockHounds",
                  "Millwall",
                  "Milwaukee Braves",
                  "Milwaukee Brewers",
                  "Milwaukee Bucks",
                  "Milwaukee Hawks",
                  "Minnesota Golden Gophers",
                  "Minnesota Lynx",
                  "Minnesota North Stars",
                  "Minnesota Timberwolves",
                  "Minnesota Twins",
                  "Minnesota United FC",
                  "Minnesota Vikings",
                  "Minnesota Wild",
                  "Mirsad Bektic",
                  "Misha Cirkunov",
                  "Mississippi Braves",
                  "Mississippi Old Miss Rebels",
                  "Mississippi State Bulldogs",
                  "Mississippi Valley State Delta Devils",
                  "Missoula Osprey",
                  "Missouri Kansas City Kangaroos",
                  "Missouri Tigers",
                  "Mito HollyHock",
                  "Mobile BayBears",
                  "Modena",
                  "Modesto Nuts",
                  "Mohun Bagan",
                  "Moldova",
                  "Monaco",
                  "Mongolia",
                  "Monmouth Hawks",
                  "Montana Grizzlies",
                  "Montana State Bobcats",
                  "Montedio Yamagata",
                  "Montenegro",
                  "Montgomery Biscuits",
                  "Montpellier",
                  "Montreal Alouettes",
                  "Montreal Canadiens",
                  "Montreal Expos",
                  "Montreal Impact",
                  "Montreal Maroons",
                  "Montreal Wanderers",
                  "Monza",
                  "Morehead State Eagles",
                  "Moreirense",
                  "Morgan State Bears",
                  "Morocco",
                  "Motherwell",
                  "Mount St. Mary's Mountaineers",
                  "Mozambique",
                  "MP Yodha",
                  "Mumbai City FC",
                  "Mumbai Indians",
                  "Mumbai Maharathi",
                  "Mumbai Rockets",
                  "Murray State Racers",
                  "Myanmar",
                  "Myrtle Beach Pelicans",
                  "NAC Breda",
                  "NAGOYA DIAMOND DOLPHINS",
                  "Nagoya Grampus Eight",
                  "Namibia",
                  "Nantes",
                  "Nashville Predators",
                  "Nashville SC",
                  "Nashville Sounds",
                  "Nate Diaz",
                  "Nauru",
                  "Navy Midshipmen",
                  "NCR Punjab Royals",
                  "Nebraska Cornhuskers",
                  "NEC Nijmegen",
                  "Necaxa",
                  "Neil Magny",
                  "Nepal",
                  "NEROCA FC",
                  "Netherlands",
                  "Nevada Wolf Pack",
                  "New Britain Rock Cats",
                  "New England Black Wolves",
                  "New England Patriots",
                  "New England Revolution",
                  "New Hampshire Fisher Cats",
                  "New Hampshire Wildcats",
                  "New Jersey Devils",
                  "New Jersey Nets",
                  "New Mexico Lobos",
                  "New Mexico State Aggies",
                  "New Orleans Pelicans",
                  "New Orleans Privateers",
                  "New Orleans Saints",
                  "New Orleans Zephyrs",
                  "New York Americans",
                  "New York City FC",
                  "New York Giants",
                  "New York Highlanders",
                  "New York Islanders",
                  "New York Jets",
                  "New York Knicks",
                  "New York Liberty",
                  "New York Mets",
                  "New York Rangers",
                  "New York Red Bulls",
                  "New York Riptide",
                  "New York Titans",
                  "New York Yankees",
                  "New Zealand",
                  "Newcastle United",
                  "Niagara Purple Eagles",
                  "Nicaragua",
                  "Nicco Montaño",
                  "Nice",
                  "Nicholls State Colonels",
                  "Niger",
                  "Nigeria",
                  "NIIGATA ALBIREX BB",
                  "Nikita Krylov",
                  "Nina Ansaroff",
                  "NISHINOMIYA STORKS",
                  "NJ/NY Gotham FC",
                  "NJIT Highlanders",
                  "Norfolk State Spartans",
                  "Norfolk Tides",
                  "North Alabama Lions",
                  "North Carolina A&T Aggies",
                  "North Carolina Asheville Bulldogs",
                  "North Carolina Central Eagles",
                  "North Carolina Charlotte 49ers",
                  "North Carolina Courage",
                  "North Carolina Greensboro Spartans",
                  "North Carolina State Wolfpack",
                  "North Carolina Tar Heels",
                  "North Carolina Wilmington Seahawks",
                  "North Dakota",
                  "North Dakota Fighting Hawks",
                  "North Dakota Fighting Sioux",
                  "North Dakota State Bison",
                  "North Eastern Warriors",
                  "North Florida Ospreys",
                  "North Korea",
                  "North Texas Mean Green",
                  "Northeast United FC",
                  "Northeastern Huskies",
                  "Northeastern Illinois Golden Eagles",
                  "Northern Arizona Lumberjacks",
                  "Northern Colorado Bears",
                  "Northern Illinois Huskies",
                  "Northern Iowa Panthers",
                  "Northern Kentucky Norse",
                  "Northwest Arkansas Naturals",
                  "Northwestern State Demons",
                  "Northwestern Wildcats",
                  "Norway",
                  "Norwich City",
                  "Notre Dame Fighting Irish",
                  "Nottingham Forest",
                  "Nurnberg",
                  "NYIT Bears",
                  "NYU Bobcats",
                  "NYU Violets",
                  "Nîmes Olympique",
                  "Oakland Athletics",
                  "Oakland Golden Grizzlies",
                  "Oakland Raiders",
                  "Odisha FC",
                  "Ogden Raptors",
                  "Ohio Bobcats",
                  "Ohio State Buckeyes",
                  "Oita Trinita",
                  "Oklahoma City RedHawks",
                  "Oklahoma City Thunder",
                  "Oklahoma Sooners",
                  "Oklahoma State Cowboys",
                  "Old Dominion Monarchs",
                  "Ole Miss Rebels",
                  "Oleksiy Oliynyk",
                  "Olympiacos Basketball",
                  "Omaha Mavericks",
                  "Omaha Royals",
                  "Oman",
                  "Omiya Ardija",
                  "Oral Roberts Golden Eagles",
                  "Oregon Ducks",
                  "Oregon State Beavers",
                  "Orem Owlz",
                  "Orix Buffaloes",
                  "Orlando City SC",
                  "Orlando Magic",
                  "Orlando Pride",
                  "OSAKA EVESSA",
                  "Osasuna",
                  "OTSUKA CORPORATION ALPHAS",
                  "Ottawa Redblacks",
                  "Ottawa Senators",
                  "Ovince Saint Preux",
                  "Pacific Boxers",
                  "Pacific FC",
                  "Pacific Tigers",
                  "Pakistan",
                  "Palau",
                  "Palermo",
                  "Palestine",
                  "Palm Beach Cardinals",
                  "Panama",
                  "Panathinaikos Basketball",
                  "Papua New Guinea",
                  "Paraguay",
                  "Parma",
                  "Parma Calcio",
                  "Patna Pirates",
                  "Patrick Thistle",
                  "Paul Felder",
                  "Paul Menard",
                  "Paulo Costa",
                  "Pawtucket Red Sox",
                  "Paços de Ferreira",
                  "Pedro Munhoz",
                  "Penn Quakers",
                  "Penn State Nittany Lions",
                  "Pennsylvania Quakers",
                  "Peoria Chiefs",
                  "Pepperdine Waves",
                  "Peru",
                  "Perugia",
                  "PGA",
                  "Philadelphia 76ers",
                  "Philadelphia Athletics",
                  "Philadelphia Eagles",
                  "Philadelphia Flyers",
                  "Philadelphia Phillies",
                  "Philadelphia Quakers",
                  "Philadelphia Union",
                  "Philadelphia Wings",
                  "Philippines",
                  "Phoenix Mercury",
                  "Phoenix Suns",
                  "Piacenza",
                  "Pisa",
                  "Pittsburgh Panthers",
                  "Pittsburgh Penguins",
                  "Pittsburgh Pirates",
                  "Pittsburgh Steelers",
                  "Plymouth Argyle",
                  "Poland",
                  "Portimonense SC",
                  "Portland Beavers",
                  "Portland Fire",
                  "Portland Pilots",
                  "Portland Sea Dogs",
                  "Portland State Vikings",
                  "Portland Thorns FC",
                  "Portland Timbers",
                  "Portland Trail Blazers",
                  "Porto",
                  "Portugal",
                  "Potomac Nationals",
                  "Prairie View Panthers",
                  "Presbyterian Blue Hose",
                  "Preston North End",
                  "Princeton Rays",
                  "Princeton Tigers",
                  "Providence Friars",
                  "PSG",
                  "PSV Eindhoven",
                  "Puerto Rico",
                  "Pulaski Mariners",
                  "Pune 7 Aces",
                  "Puneri Paltan",
                  "Punjab FC",
                  "Purdue Boilermakers",
                  "Qatar",
                  "QPR",
                  "Quad Cities River Bandits",
                  "Querétaro",
                  "Quess East Bengal",
                  "Quinnipiac Bobcats",
                  "Racing Louisville FC",
                  "Racing Santander",
                  "Radford Highlanders",
                  "Rafael dos Anjos",
                  "Rajasthan Royals",
                  "Ranchi Rays",
                  "Rancho Cucamonga Quakes",
                  "Randa Markos",
                  "Rangers",
                  "Rani Yahya",
                  "Raphael Assunção",
                  "Raquel Pennington",
                  "Ray Borg",
                  "Rayo Vallecano",
                  "RB Leipzig",
                  "RBC Roosendaal",
                  "Reading",
                  "Reading Phillies",
                  "Real Kashmir FC",
                  "Real Madrid",
                  "Real Madrid Basketball",
                  "Real Oviedo",
                  "Real Salt Lake",
                  "Real Sociedad",
                  "Real Zaragoza",
                  "Recreativo Huelva",
                  "Red Bull Racing",
                  "Refugee Olympic Team",
                  "Reggina",
                  "Renato Moicano",
                  "Renault DP World",
                  "Rennes",
                  "Reno Aces",
                  "RENOFA Yamaguchi",
                  "Rhode Island Rams",
                  "Ricardo Lamas",
                  "Rice Owls",
                  "Richard Petty",
                  "Richmond Flying Squirrels",
                  "Richmond Spiders",
                  "Ricky Stenhouse Jr.",
                  "Rider Broncs",
                  "Rio Ave",
                  "Rising Pune Supergiants",
                  "RIZING ZEPHYR FUKUOKA",
                  "RKC Waalwijk",
                  "Roasso Kumamoto",
                  "Rob Font",
                  "Robbie Lawler",
                  "Robert Morris Colonials",
                  "Robert Whittaker",
                  "Rochester Knighthawks",
                  "Rochester Red Wings",
                  "Rochester Royals",
                  "Roda JC Kerkrade",
                  "Roma",
                  "Romania",
                  "Rome Braves",
                  "Rose Namajunas",
                  "Ross County",
                  "Rotherham United",
                  "Round Rock Express",
                  "Roxanne Modafferi",
                  "Royal Challengers Bangalore",
                  "Russia",
                  "Rutgers Scarlet Knights",
                  "Rwanda",
                  "Ryan Blaney",
                  "Ryan Newman",
                  "RYUKYU GOLDEN KINGS",
                  "Sacramento Kings",
                  "Sacramento Monarchs",
                  "Sacramento River Cats",
                  "Sacred Heart Pioneers",
                  "Sagan Tosu",
                  "Saint Kitts and Nevis",
                  "Saint Lucia",
                  "Saint Mary's Gaels",
                  "Saint Vincent and the Grenadines",
                  "SAITAMA BRONCOS",
                  "Saitama Seibu Lions",
                  "Salem Red Sox",
                  "Salem-Keizer Volcanoes",
                  "Salt Lake Bees",
                  "Sam Houston State Bearkats",
                  "Samford Bulldogs",
                  "Samoa",
                  "Sampdoria",
                  "San Antonio Missions",
                  "San Antonio Silver Stars",
                  "San Antonio Spurs",
                  "San Diego Chargers",
                  "San Diego Clippers",
                  "San Diego Padres",
                  "San Diego Rockets",
                  "San Diego Seals",
                  "San Diego State Aztecs",
                  "San Diego Toreros",
                  "San Diego Wave FC",
                  "San Francisco 49ers",
                  "San Francisco Dons",
                  "San Francisco Giants",
                  "San Francisco Warriors",
                  "San Jose Earthquakes",
                  "San Jose Giants",
                  "San Jose Sharks",
                  "San Jose State Spartans",
                  "San Marino",
                  "SAN-EN NEOPHOENIX",
                  "Sanfrecce Hiroshima",
                  "Santa Clara Broncos",
                  "Santiago Ponzinibbio",
                  "Sao Paulo FC",
                  "Sara McMann",
                  "Saskatchewan Roughriders",
                  "Saskatchewan Rush",
                  "Sassuolo",
                  "Saudi Arabia",
                  "Savannah Sand Gnats",
                  "Savannah State Tigers",
                  "SC Cambuur",
                  "SC Sagamihara",
                  "Schalke",
                  "Scotland",
                  "Scranton/Wilkes-Barre Yankees",
                  "Scuderia AlphaTauri",
                  "Scuderia Ferrari",
                  "SD Eibar",
                  "SD Huesca",
                  "SD Ponferradina",
                  "SEAHORSES MIKAWA",
                  "Seattle Kraken",
                  "Seattle Mariners",
                  "Seattle Redhawks",
                  "Seattle Reign FC",
                  "Seattle Seahawks",
                  "Seattle Sounders FC",
                  "Seattle Storm",
                  "Seattle SuperSonics",
                  "Sedan",
                  "SENDAI EIGHTY NINERS",
                  "Senegal",
                  "Serbia",
                  "Serbia and Montenegro",
                  "Sergio Pettis",
                  "Seton Hall Pirates",
                  "Seychelles",
                  "Shamil Abdurakhimov",
                  "Sheffield United",
                  "Sheffield Wednesday",
                  "SHIGA LAKESTARS",
                  "SHIMANE SUSANOO MAGIC",
                  "Shimizu S-Pulse",
                  "SHINSHU BRAVE WARRIORS",
                  "Shonan Bellmare",
                  "Siena Saints",
                  "Sierra Leone",
                  "Sijara Eubanks",
                  "Singapore",
                  "SIU Edwardsville Cougars",
                  "Sky Blue FC",
                  "Slovakia",
                  "Slovenia",
                  "SM Caen",
                  "SMU Mustangs",
                  "Sochaux",
                  "Solomon Islands",
                  "Somalia",
                  "South Africa",
                  "South Alabama Jaguars",
                  "South Bend Silver Hawks",
                  "South Carolina Fighting Gamecocks",
                  "South Carolina State Bulldogs",
                  "South Dakota Coyotes",
                  "South Dakota State Jackrabbits",
                  "South Florida Bulls",
                  "South Korea",
                  "South Sudan",
                  "Southampton",
                  "Southeast Missouri State Indians",
                  "Southeast Missouri State Redhawks",
                  "Southeastern Louisiana Lions",
                  "Southern Illinois Salukis",
                  "Southern Jaguars",
                  "Southern Mississippi Golden Eagles",
                  "Southern Utah Thunderbirds",
                  "Southwest Missouri State Bears",
                  "Spain",
                  "Spal",
                  "Sparta Rotterdam",
                  "Spokane Indians",
                  "Sport Club Corinthians Paulista",
                  "Sport-Club Freiburg",
                  "Sporting",
                  "Sporting de Braga",
                  "Sporting Gijón",
                  "Sporting Kansas City",
                  "Springfield Cardinals",
                  "Sri Lanka",
                  "SSC Napoli",
                  "St Johnstone",
                  "St Mirren",
                  "St. Bonaventure Bonnies",
                  "St. Francis (New York) Terriers",
                  "St. Francis (Pennsylvania) Red Flash",
                  "St. Francis Brooklyn Terriers",
                  "St. John's Red Storm",
                  "St. Joseph's Hawks",
                  "St. Louis Blues",
                  "St. Louis Bombers",
                  "St. Louis Cardinals",
                  "St. Louis City",
                  "St. Louis Eagles",
                  "St. Louis Hawks",
                  "St. Louis Rams",
                  "St. Louis University Billikens",
                  "St. Lucie Mets",
                  "St. Mary's Rattlers",
                  "St. Peter's Peacocks",
                  "Stade de Reims",
                  "Stanford Cardinal",
                  "State College Spikes",
                  "Staten Island Yankees",
                  "Stefan Struve",
                  "Stephen F. Austin Lumberjacks",
                  "Stephen Thompson",
                  "Stetson Hatters",
                  "Stipe Miocic",
                  "Stockton Ports",
                  "Stoke City",
                  "Stony Brook Seawolves",
                  "Strasbourg",
                  "Sudan",
                  "Sunderland",
                  "Sunrisers Hyderabad",
                  "SUNROCKERS SHIBUYA",
                  "Suriname",
                  "Swansea City",
                  "Swaziland",
                  "Sweden",
                  "Switzerland",
                  "Syracuse Chiefs",
                  "Syracuse Nationals",
                  "Syracuse Orange",
                  "Syria",
                  "São Tomé and Príncipe",
                  "Tacoma Rainiers",
                  "Tai Tuivasa",
                  "Tajikistan",
                  "Tamil Thalaivas",
                  "Tampa Bay Buccaneers",
                  "Tampa Bay Lightning",
                  "Tampa Bay Rays",
                  "Tampa Rays",
                  "Tampa Yankees",
                  "Tanzania",
                  "Tatiana Suarez",
                  "TCU Horned Frogs",
                  "Team Cuba",
                  "Team Dominican Republic",
                  "Team Japan",
                  "Team Netherlands",
                  "Team Panama",
                  "Team Puerto Rico",
                  "Team South Korea",
                  "Team United States",
                  "Team Venezuela",
                  "Tecia Torres",
                  "Telugu Titans",
                  "Temple Owls",
                  "Tennessee Chattanooga Mocs",
                  "Tennessee Martin Skyhawks",
                  "Tennessee Smokies",
                  "Tennessee State Tigers",
                  "Tennessee Tech Golden Eagles",
                  "Tennessee Titans",
                  "Tennessee Volunteers",
                  "Tennis",
                  "Ternana",
                  "Texas A&M Aggies",
                  "Texas A&M-Corpus Christi Islanders",
                  "Texas Arlington Mavericks",
                  "Texas El Paso Miners",
                  "Texas Longhorns",
                  "Texas Pan American Broncs",
                  "Texas Rangers",
                  "Texas San Antonio Roadrunners",
                  "Texas Southern Tigers",
                  "Texas State Bobcats",
                  "Texas Tech Red Raiders",
                  "Texas-Rio Grande Valley Vaqueros",
                  "Thailand",
                  "The Gambia",
                  "Thespakusatsu Gunma",
                  "Thiago Santos",
                  "Thomas Almeida",
                  "Thonon Evian FC",
                  "Tiddim Road Athletic Union",
                  "Tim Elliott",
                  "TJ Dillashaw",
                  "TOCHIGI BREX",
                  "Tochigi SC",
                  "Togo",
                  "Tohoku Rakuten Golden Eagles",
                  "TOKIO MARINE NICHIDO BIG BLUE",
                  "Tokushima Vortis",
                  "TOKYO CINQ REVES",
                  "TOKYO EXCELLENCE",
                  "TOKYO HACHIOJI TRAINS",
                  "Tokyo Verdy1969",
                  "Tokyo Yakult Swallows",
                  "Toledo Mud Hens",
                  "Toledo Rockets",
                  "Tondela",
                  "Tonga",
                  "Tony Ferguson",
                  "Tony Stewart",
                  "Tonya Evinger",
                  "Torino",
                  "Toronto Arenas",
                  "Toronto Argonauts",
                  "Toronto Blue Jays",
                  "Toronto FC",
                  "Toronto Maple Leafs",
                  "Toronto Raptors",
                  "Toronto Rock",
                  "Toronto St. Pats",
                  "Toronto Tempo",
                  "Tottenham Hotspur",
                  "Toulouse FC",
                  "Towson Tigers",
                  "TOYAMA GROUSES",
                  "TOYODA GOSEI SCORPIONS",
                  "Trenton Thunder",
                  "Trevor Bayne",
                  "Tri-City Dust Devils",
                  "Tri-City ValleyCats",
                  "Trinidad and Tobago",
                  "Troy State Trojans",
                  "Troyes",
                  "TSG 1899 Hoffenheim",
                  "TSV 1860 Munich",
                  "Tulane Green Wave",
                  "Tulsa Drillers",
                  "Tulsa Golden Hurricane",
                  "Tulsa Shock",
                  "Tunisia",
                  "Turkey",
                  "Turkmenistan",
                  "Tuvalu",
                  "Twente Enschede",
                  "Ty Dillon",
                  "Tyron Woodley",
                  "Tyson Pedro",
                  "U Mumba",
                  "U Mumba Volley",
                  "UANL Tigres",
                  "UC Davis Aggies",
                  "UCLA Bruins",
                  "UD Almería",
                  "UD Las Palmas",
                  "Udinese",
                  "Uganda",
                  "Ukraine",
                  "Ulka Sasaki",
                  "UMass Lowell River Hawks",
                  "Union Berlin",
                  "United Arab Emirates",
                  "United States",
                  "UNLV Rebels",
                  "UP Dangal",
                  "UP Yoddha",
                  "Urawa Red Diamonds",
                  "Uriah Hall",
                  "Uruguay",
                  "US Salernitana",
                  "USC Trojans",
                  "USC Upstate Spartans",
                  "Utah Jazz",
                  "Utah Mammoth",
                  "Utah Royals FC",
                  "Utah State Aggies",
                  "Utah Utes",
                  "Utah Valley Wolverines",
                  "Uttar Pradesh Wizards",
                  "Uzbekistan",
                  "V-Varen Nagasaki",
                  "Valencia",
                  "Valencia Basketball",
                  "Valenciennes FC",
                  "Valentina Shevchenko",
                  "Valladolid",
                  "Valour FC",
                  "Valparaiso Crusaders",
                  "Vancouver Canadians",
                  "Vancouver Canucks",
                  "Vancouver FC",
                  "Vancouver Warriors",
                  "Vancouver Whitecaps",
                  "Vanderbilt Commodores",
                  "Vanuatu",
                  "Vegalta Sendai",
                  "Vegas Golden Knights",
                  "Venezia FC",
                  "Venezuela",
                  "Ventforet Kofu",
                  "Vermont Catamounts",
                  "Vermont Lake Monsters",
                  "Verona FC",
                  "VfB Stuttgart",
                  "VfL Bochum",
                  "VfL Osnabrück",
                  "VfL Wolfsburg",
                  "Vietnam",
                  "Villanova Wildcats",
                  "Villareal",
                  "Virgin Islands",
                  "Virginia Cavaliers",
                  "Virginia Commonwealth Rams",
                  "Virginia Tech Hokies",
                  "Visalia Rawhide",
                  "Vissel Kobe",
                  "Vitesse Arnhem",
                  "Vitória Guimarães",
                  "Vitória Setúbal",
                  "VMI Keydets",
                  "Volkan Oezdemir",
                  "Wagner Seahawks",
                  "Wake Forest Demon Deacons",
                  "Wales",
                  "Washington Capitals",
                  "Washington Commanders",
                  "Washington Football Team",
                  "Washington Huskies",
                  "Washington Mystics",
                  "Washington Nationals",
                  "Washington Spirit",
                  "Washington State Cougars",
                  "Washington Wizards",
                  "Watford",
                  "Weber State Wildcats",
                  "Werder Bremen",
                  "West Bromwich Albion",
                  "West Ham United",
                  "West Indies",
                  "West Michigan Whitecaps",
                  "West Tenn Diamond Jaxx",
                  "West Virginia Mountaineers",
                  "West Virginia Power",
                  "Western Carolina Catamounts",
                  "Western Illinois Leathernecks",
                  "Western Kentucky Hilltoppers",
                  "Western Michigan Broncos",
                  "Wichita State Shockers",
                  "Wigan",
                  "Willem II Tilburg",
                  "William & Mary Tribe",
                  "William Byron",
                  "Williams Racing",
                  "Williamsport Crosscutters",
                  "Wilmington Blue Rocks",
                  "Wilson Reis",
                  "Winnipeg Blue Bombers",
                  "Winnipeg Jets",
                  "Winston-Salem Dash",
                  "Winthrop Eagles",
                  "Wisconsin Badgers",
                  "Wisconsin Green Bay Phoenix",
                  "Wisconsin Milwaukee Panthers",
                  "Wisconsin Timber Rattlers",
                  "Wofford Terriers",
                  "Wolverhampton Wanderers",
                  "Wright State Raiders",
                  "WUSA",
                  "WWE",
                  "Wyoming Cowboys",
                  "X-Games",
                  "Xavier Musketeers",
                  "Yair Rodriguez",
                  "Yakima Bears",
                  "Yale Bulldogs",
                  "YAMAGATA WYVERNS",
                  "Yana Kunitskaya",
                  "Yemen",
                  "Yoel Romero",
                  "YOKOHAMA B-CORSAIRS",
                  "Yokohama DeNA BayStars",
                  "Yokohama F. Marinos",
                  "Yokohama FC",
                  "Yomiuri Giants",
                  "York United FC",
                  "Youngstown State Penguins",
                  "YSCC Yokohama",
                  "Yugoslavia",
                  "Zabit Magomedsharipov",
                  "Zalgiris Kaunas Basketball",
                  "Zambia",
                  "Zenit St Petersburg Basketball",
                  "Zimbabwe",
                  "Zweigen Kanazawa"
                ]
              }
            ],
            "title": "Team Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "Seattle Seahawks"
            ],
            "maxLength": 100,
            "description": "Please enter the team name of this product",
            "maxUtf8ByteLength": 50
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Team Name",
      "examples": [
        "Seattle Seahawks"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "deprecated": true,
      "description": "Please enter the team name of this product",
      "maxUniqueItems": 2,
      "minUniqueItems": 1
    },
    "list_price": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "currency",
          "value"
        ],
        "properties": {
          "value": {
            "type": "number",
            "title": "List Price",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "64"
            ],
            "maxLength": 20,
            "multipleOf": 0.01,
            "description": "Provide the list price for the product not including tax. List Price is the suggested retail price of a product as provided by a manufacturer, supplier, or seller. This is not the offering or cost price. If you are unable to provide a value, enter 0."
          },
          "currency": {
            "enum": [
              "USD"
            ],
            "type": "string",
            "title": "List Price Currency",
            "hidden": true,
            "editable": false,
            "examples": [
              "USD"
            ],
            "enumNames": [
              "USD"
            ],
            "description": "Select the corresponding currency"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "List Price",
      "examples": [
        "64 USD, 69 GBP, 98 EUR"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "currency"
      ],
      "description": "Provide the list price for the product. List Price is the suggested retail price of a product as provided by a manufacturer, supplier, or seller. This is not the offering or cost price.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "map_policy": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "policy_1",
              "policy_10",
              "policy_11",
              "policy_2",
              "policy_3",
              "policy_4",
              "policy_5",
              "policy_6",
              "policy_7",
              "policy_8",
              "policy_9"
            ],
            "type": "string",
            "title": "Minimum Advertised Price Display",
            "hidden": false,
            "editable": true,
            "examples": [
              "Policy 9"
            ],
            "enumNames": [
              "Policy 1",
              "Policy 10",
              "Policy 11",
              "Policy 2",
              "Policy 3",
              "Policy 4",
              "Policy 5",
              "Policy 6",
              "Policy 7",
              "Policy 8",
              "Policy 9"
            ],
            "description": "Select one."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Minimum Advertised Price Display",
      "examples": [
        "Policy 9"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Select one.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "model_name": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Model Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "MacBook Pro"
            ],
            "maxLength": 85,
            "minLength": 0,
            "description": "Specify the model name of the product as defined by the manufacturer or brand excluding item type, color, brand or size"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Model Name",
      "examples": [
        "MacBook Pro"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Specify the model name of the product as defined by the manufacturer or brand excluding item type, color, brand or size",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "skip_offer": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Skip Offer",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Please indicate whether the offer should be skipped and a buyable offer should not be created. A value of \"Yes\", means no offer will be created."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Skip Offer",
      "examples": [
        "Yes"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Please indicate whether the offer should be skipped and a buyable offer should not be created. A value of \"Yes\", means no offer will be created.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "unit_count": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "type": {
            "type": "object",
            "title": "Unit Count Type",
            "examples": [
              "Ounces"
            ],
            "required": [
              "language_tag",
              "value"
            ],
            "properties": {
              "value": {
                "type": "string",
                "title": "Unit Count Type",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Ounces"
                ],
                "maxLength": 100,
                "description": "For items consumed by volume, weight, linear dimension etc., provide the unit of measure listed on the products. For products consumed as individual units, enter: count",
                "maxUtf8ByteLength": 20
              },
              "language_tag": {
                "$ref": "#/$defs/language_tag"
              }
            },
            "description": "For items consumed by volume, weight, linear dimension etc., provide the unit of measure listed on the products. For products consumed as individual units, enter: count",
            "additionalProperties": false
          },
          "value": {
            "type": "number",
            "title": "Unit Count",
            "hidden": false,
            "editable": true,
            "examples": [
              "72.0"
            ],
            "description": "For products that are consumed by volume, weight, linear dimension, etc., provide the net quantity that would be shipped to a customer who orders one ASIN (e.g. 12 pack of 6 floz. bottles of water = 72, vs. a single 2 liter bottle = 2). For products consumed as individual units, provide the total number of units (pack of 12 pens = 12). For packed assortments of non-identical items, enter 1"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Unit Count",
      "examples": [
        "72.0 Ounces"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Specify the number of units and the unit type of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_weight": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "unit",
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "pounds"
            ],
            "type": "string",
            "title": "Item Weight Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Pounds"
            ],
            "enumNames": [
              "Pounds"
            ],
            "description": "Provide unit for item weight"
          },
          "value": {
            "type": "number",
            "title": "Item Weight",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "30.0, 1.5"
            ],
            "maxLength": 5000,
            "description": "Provide the item weight numeric value (not including the packaging)"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Weight",
      "examples": [
        "30.0 Pounds, 1.5 Kilograms"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the weight of the item (not including the packaging)",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "league_name": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Canadian Football League",
                  "Canadian Premier League",
                  "Dutch Soccer",
                  "E-Sports",
                  "English Soccer",
                  "European Basketball",
                  "Formula 1",
                  "French Soccer",
                  "German Soccer",
                  "Hockey India League",
                  "I-League",
                  "Indian Premier League",
                  "Indian Soccer League",
                  "International Cricket",
                  "Italian Soccer",
                  "Japanese Baseball",
                  "Japanese Basketball",
                  "Japanese Soccer",
                  "LPGA",
                  "Mexican Football Federation",
                  "Minor League Baseball",
                  "MLB",
                  "MLS",
                  "NASCAR",
                  "National Lacrosse League",
                  "National Teams",
                  "NBA",
                  "NCAA",
                  "NFL",
                  "NHL",
                  "NWSL",
                  "Other Soccer Leagues",
                  "PGA",
                  "Portuguese Soccer",
                  "Premier Badminton League",
                  "Pro Kabaddi League",
                  "Pro Volleyball League",
                  "Pro Wrestling League",
                  "Scottish Soccer",
                  "Spanish Soccer",
                  "Tennis",
                  "UFC",
                  "WNBA",
                  "World Baseball Classic",
                  "World Cup Soccer",
                  "WUSA",
                  "WWE",
                  "X-Games"
                ],
                "type": "string",
                "enumNames": [
                  "Canadian Football League",
                  "Canadian Premier League",
                  "Dutch Soccer",
                  "E-Sports",
                  "English Soccer",
                  "European Basketball",
                  "Formula 1",
                  "French Soccer",
                  "German Soccer",
                  "Hockey India League",
                  "I-League",
                  "Indian Premier League",
                  "Indian Soccer League",
                  "International Cricket",
                  "Italian Soccer",
                  "Japanese Baseball",
                  "Japanese Basketball",
                  "Japanese Soccer",
                  "LPGA",
                  "Mexican Football Federation",
                  "Minor League Baseball",
                  "MLB",
                  "MLS",
                  "NASCAR",
                  "National Lacrosse League",
                  "National Teams",
                  "NBA",
                  "NCAA",
                  "NFL",
                  "NHL",
                  "NWSL",
                  "Other Soccer Leagues",
                  "PGA",
                  "Portuguese Soccer",
                  "Premier Badminton League",
                  "Pro Kabaddi League",
                  "Pro Volleyball League",
                  "Pro Wrestling League",
                  "Scottish Soccer",
                  "Spanish Soccer",
                  "Tennis",
                  "UFC",
                  "WNBA",
                  "World Baseball Classic",
                  "World Cup Soccer",
                  "WUSA",
                  "WWE",
                  "X-Games"
                ]
              }
            ],
            "title": "League Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "NBA"
            ],
            "maxLength": 100,
            "description": "Provide the league name associated with this product",
            "maxUtf8ByteLength": 50
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "League Name",
      "examples": [
        "NBA"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "deprecated": true,
      "description": "Name of league associated with this event",
      "maxUniqueItems": 6,
      "minUniqueItems": 1
    },
    "part_number": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Part Number",
            "hidden": false,
            "editable": true,
            "examples": [
              "RIV001"
            ],
            "maxLength": 40,
            "minLength": 0,
            "description": "Provide the part number. For many products, this will be identical to the model number however some manufacturers distinguish part number from model number"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Manufacturer Part Number",
      "examples": [
        "LE"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "For most products, this will be identical to the model number; however, some manufacturers distinguish part number from model number.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "bullet_point": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Bullet Point",
            "hidden": false,
            "editable": true,
            "examples": [
              "Breathable Leather Lining"
            ],
            "maxLength": 550,
            "minLength": 0,
            "description": "Brief descriptive text, called out via a bullet point, regarding a specific aspect of the product. These display directly under or next to your product photo, it is useful to put interesting information in these fields. Do NOT use all caps or abbreviations. Please do NOT use for fabric content, care instructions or country as these are populated in different fields."
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Key Product Features",
      "examples": [
        "Delicious honey-apricot glaze"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Max. 100 characters per line. Use these to highlight some of the product's most important qualities. Each line will be displayed as a separate bullet point above the product description.",
      "maxUniqueItems": 10,
      "minUniqueItems": 1
    },
    "gift_options": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "can_be_wrapped": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Is Gift Wrap Available",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "If you can gift wrap an item indicate that here.  If left blank, defaults to 'No'"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "can_be_messaged": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Offering Can Be Gift Messaged",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "If you can print a gift message with the item indicate that here. If left blank, defaults to 'No'"
          }
        },
        "additionalProperties": false
      },
      "title": "Gift Options",
      "examples": [
        "Yes"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide gift card options",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "manufacturer": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Manufacturer",
            "hidden": false,
            "editable": false,
            "examples": [
              "Nike, Procter & Gamble"
            ],
            "maxLength": 100,
            "minLength": 0,
            "description": "Provide the company that manufactures the product."
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Manufacturer",
      "examples": [
        "Sony, Kitchen Aid, Microsoft"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "The full name of the publisher who issued the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "model_number": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Model Number",
            "hidden": false,
            "editable": true,
            "examples": [
              "RXZER23"
            ],
            "maxLength": 40,
            "minLength": 0,
            "description": "Provide the manufacturer 's model number for the item",
            "maxUtf8ByteLength": 40
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Model Number",
      "examples": [
        "C-50"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Product code assigned by the manufacturer; can be numbers, letters, or both",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "contains_pfas": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Contains PFAS",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Provide whether the item contains PFAS (perfluoroalkyl or polyfluoroalkyl substances), a common but complex group of synthetic chemicals."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Contains PFAS",
      "examples": [
        "Yes"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide whether the item contains PFAS (perfluoroalkyl or polyfluoroalkyl substances), a common but complex group of synthetic chemicals.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "num_batteries": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "quantity",
          "type"
        ],
        "properties": {
          "type": {
            "enum": [
              "12v",
              "9v",
              "a",
              "aa",
              "aaa",
              "aaaa",
              "c",
              "cr123a",
              "cr2",
              "cr2032",
              "cr2430",
              "cr5",
              "d",
              "lithium_ion",
              "lithium_metal",
              "lithium_polymer",
              "lr41",
              "lr43",
              "lr44",
              "nonstandard_battery",
              "p76",
              "product_specific",
              "unknown"
            ],
            "type": "string",
            "title": "Battery Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "12V"
            ],
            "enumNames": [
              "12V",
              "9V",
              "A",
              "AA",
              "AAA",
              "AAAA",
              "C",
              "CR123A",
              "CR2",
              "CR2032",
              "CR2430",
              "CR5",
              "D",
              "Lithium Ion",
              "Lithium Metal",
              "Lithium Polymer",
              "LR41",
              "LR43",
              "LR44",
              "Nonstandard Battery",
              "P76",
              "Product Specific",
              "Unknown"
            ],
            "description": "Provide battery type needed to power the item, including spares if included. Some options may be moved under other attribute eg. IEC code"
          },
          "quantity": {
            "type": "integer",
            "title": "Number of Batteries",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "1, 4"
            ],
            "description": "Specify the number of batteries needed to power the item.  If batteries are included with the item be sure to account for spare batteries provided"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Number of Batteries",
      "examples": [
        "1 AA, 2 AAA"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "type"
      ],
      "description": "Provide the quantity and type of batteries needed to power the item.  If batteries are included with the item be sure to account for spare batteries provided",
      "maxUniqueItems": 1000,
      "minUniqueItems": 1
    },
    "package_level": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "case",
              "pallet",
              "unit"
            ],
            "type": "string",
            "title": "Package Level",
            "hidden": false,
            "editable": true,
            "examples": [
              "Unit, Case"
            ],
            "enumNames": [
              "Case",
              "Pallet",
              "Unit"
            ],
            "description": "Provide the package level of the item. Choose “Unit” when package hierarchy is not provided or applicable. Provide one “Unit” item for every package hierarchy."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Package Level",
      "examples": [
        "Unit, Case"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the package level of the item. Choose “Unit” when package hierarchy is not provided or applicable. Provide one “Unit” item for every package hierarchy.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "condition_note": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Offer Condition Note",
            "hidden": false,
            "editable": true,
            "examples": [
              "Small dent in left side panel."
            ],
            "maxLength": 2204,
            "description": "Provide descriptive text explaining the actual condition of the item"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Offer Condition Note",
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide descriptive text explaining the actual condition of the item",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "condition_type": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "club_club",
              "collectible_acceptable",
              "collectible_good",
              "collectible_like_new",
              "collectible_very_good",
              "new_new",
              "new_oem",
              "new_open_box",
              "refurbished_refurbished",
              "used_acceptable",
              "used_good",
              "used_like_new",
              "used_very_good"
            ],
            "type": "string",
            "title": "Item Condition",
            "hidden": false,
            "editable": false,
            "examples": [
              "New"
            ],
            "enumNames": [
              "Club",
              "Collectible - Acceptable",
              "Collectible - Good",
              "Collectible - Like New",
              "Collectible - Very Good",
              "New",
              "New - OEM",
              "New - Open Box",
              "Refurbished",
              "Used - Acceptable",
              "Used - Good",
              "Used - Like New",
              "Used - Very Good"
            ],
            "description": "Provide the actual condition type of the product"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Condition",
      "examples": [
        "New"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the actual condition type of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "control_method": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "application",
              "gesture",
              "push_button",
              "remote",
              "touch",
              "voice"
            ],
            "type": "string",
            "title": "Control Method",
            "hidden": false,
            "editable": true,
            "examples": [
              "App"
            ],
            "enumNames": [
              "App",
              "Gesture",
              "Push Button",
              "Remote",
              "Touch",
              "Voice"
            ],
            "description": "Provide the mechanism used to control the item for standard operations."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Control Method",
      "examples": [
        "App"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the mechanism used to control the item for standard operations.",
      "maxUniqueItems": 4,
      "minUniqueItems": 1
    },
    "ships_globally": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Ships Globally",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Provide whether the item can be shipped globally by Amazon "
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Ships Globally",
      "examples": [
        "Yes"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide whether the item can be shipped globally by Amazon ",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "generic_keyword": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Generic Keyword",
            "hidden": false,
            "editable": true,
            "examples": [
              "Water sport shoes; Derek Rose; Electric; Wi-Fi; Banana"
            ],
            "maxLength": 500,
            "minLength": 0,
            "description": "Provide any terms that may be relevant to customer searches. No repetition, no competitor brand names or ASINs.",
            "maxUtf8ByteLength": 2000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Search Terms",
      "examples": [
        "Dark Chocolate, Apples, Cookies"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide specific search terms to help customers find your product.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "lithium_battery": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "weight": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "unit",
                "value"
              ],
              "properties": {
                "unit": {
                  "enum": [
                    "grams",
                    "kilograms",
                    "milligrams",
                    "ounces",
                    "pounds"
                  ],
                  "type": "string",
                  "title": "Lithium Battery Weight Unit",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "Grams"
                  ],
                  "enumNames": [
                    "Grams",
                    "Kilograms",
                    "Milligrams",
                    "Ounces",
                    "Pounds"
                  ],
                  "description": "Select the corresponding weight unit"
                },
                "value": {
                  "type": "number",
                  "title": "Lithium Battery Weight",
                  "hidden": false,
                  "minimum": 0,
                  "editable": true,
                  "examples": [
                    "0.5, 0.03"
                  ],
                  "maxLength": 12,
                  "description": "Provide the weight of lithium contained in the cell or battery as a numeric value"
                }
              },
              "additionalProperties": false
            },
            "title": "Lithium Battery Weight",
            "examples": [
              "0.5 grams, 0.03 grams"
            ],
            "maxItems": 1,
            "minItems": 1,
            "description": "Provide the weight of lithium contained in the cell or battery"
          },
          "packaging": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "value"
              ],
              "properties": {
                "value": {
                  "enum": [
                    "batteries_contained_in_equipment",
                    "batteries_only",
                    "batteries_packed_with_equipment"
                  ],
                  "type": "string",
                  "title": "Lithium Battery Packaging",
                  "hidden": false,
                  "editable": true,
                  "examples": [
                    "Batteries contained in equipment, Batteries packed with equipment, Batteries only"
                  ],
                  "enumNames": [
                    "Batteries contained in equipment",
                    "Batteries only",
                    "Batteries packed with equipment"
                  ],
                  "description": "Select “in equipment” if the battery is contained in the item . Select “with equipment” if the battery is packed separately with the device it is meant to power. Select “only” if the product is a battery sold alone or with items it is not meant to power."
                }
              },
              "additionalProperties": false
            },
            "title": "Lithium Battery Packaging",
            "maxItems": 1,
            "minItems": 1,
            "description": "Choices are \"batteries_only\" (If battery is a standalone) \"batteries_contained_in_equipment\" (if battery is assembled in the item) or \"batteries_packed_with_equipment\" (If battery is included in the item packaging but not assembled in the item)"
          },
          "energy_content": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "unit",
                "value"
              ],
              "properties": {
                "unit": {
                  "enum": [
                    "btus",
                    "cubic_feet",
                    "cubic_meters",
                    "joules",
                    "kilowatt_hours",
                    "milliamp_hours",
                    "milliampere_hour",
                    "milliampere_second",
                    "watt_hours"
                  ],
                  "type": "string",
                  "title": "Lithium Battery Energy Content Unit",
                  "hidden": false,
                  "editable": false,
                  "examples": [
                    "Watt Hours"
                  ],
                  "enumNames": [
                    "British Thermal Units (BTUs)",
                    "Cubic Feet",
                    "Cubic Meters",
                    "Joules",
                    "Kilowatt Hours",
                    "Milliamp Hours (mAh)",
                    "Milliampere Hour (mAh)",
                    "Milliampere Second (mAs)",
                    "Watt Hours"
                  ],
                  "description": "Select the corresponding unit"
                },
                "value": {
                  "type": "number",
                  "title": "Lithium Battery Energy Content",
                  "hidden": false,
                  "minimum": 0,
                  "editable": false,
                  "examples": [
                    "2.6"
                  ],
                  "maxLength": 5000,
                  "description": "Provide the total energy stored in the lithium batteries used to power the item, measured in Watt Hours."
                }
              },
              "additionalProperties": false
            },
            "title": "Lithium Battery Energy Content",
            "maxItems": 1,
            "minItems": 1,
            "description": "Watt hours of each battery (or cell) in unit"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Lithium Battery",
      "examples": [
        "Milligrams"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Lithium Battery of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "number_of_items": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Number of Items",
            "hidden": false,
            "maximum": 999999999999,
            "minimum": 0,
            "editable": true,
            "examples": [
              "5"
            ],
            "description": "Provide the total number of identical items in the selling unit to the customer"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Number of Items",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the total number of identical items in the selling unit to the customer",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "parentage_level": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "child",
              "parent"
            ],
            "type": "string",
            "title": "Parentage Level",
            "hidden": false,
            "editable": true,
            "examples": [
              "Parent"
            ],
            "enumNames": [
              "Child",
              "Parent"
            ],
            "description": "Specify whether a SKU is a parent or child"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Parentage Level",
      "examples": [
        "Parent"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Specify whether a SKU is a parent or child",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "variation_theme": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "name"
        ],
        "properties": {
          "name": {
            "enum": [
              "COLOR",
              "COLOR/MATERIAL",
              "COLOR/NUMBER_OF_ITEMS",
              "COLOR/SIZE",
              "COLOR/WATTAGE",
              "COLOR_NAME",
              "COLOR_NAME/ITEM_DISPLAY_WEIGHT",
              "COLOR_NAME/MATERIAL_TYPE",
              "COLOR_NAME/NUMBER_OF_ITEMS",
              "COLOR_NAME/SIZE_NAME",
              "COLOR_NAME/SIZE_NAME/STYLE_NAME",
              "COLOR_NAME/STYLE_NAME",
              "COLOR_NAME/WATTAGE",
              "CUSTOMER_PACKAGE_TYPE",
              "FLAVOR/SIZE",
              "FLAVOR_NAME",
              "ITEM_DISPLAY_WEIGHT",
              "ITEM_DISPLAY_WEIGHT/COLOR_NAME",
              "ITEM_DISPLAY_WEIGHT/MATERIAL_TYPE",
              "ITEM_DISPLAY_WEIGHT/SIZE_NAME",
              "ITEM_PACKAGE_QUANTITY",
              "ITEM_PACKAGE_QUANTITY/COLOR_NAME",
              "ITEM_PACKAGE_QUANTITY/SIZE_NAME",
              "ITEM_PACKAGE_QUANTITY/STYLE_NAME",
              "ITEM_WEIGHT",
              "MATERIAL/COLOR",
              "MATERIAL/SIZE",
              "MATERIAL_TYPE",
              "MATERIAL_TYPE/COLOR_NAME",
              "MATERIAL_TYPE/ITEM_DISPLAY_WEIGHT",
              "MATERIAL_TYPE/SIZE_NAME",
              "MODEL",
              "MODEL/SIZE_NAME",
              "MODEL_NAME",
              "MODEL_NAME/TEAM_NAME",
              "MODEL_NUMBER/SIZE",
              "NUMBER_OF_ITEMS",
              "PATTERN",
              "PATTERN_NAME",
              "PATTERN_NAME/SIZE_NAME",
              "SIZE",
              "SIZE/COLOR",
              "SIZE/COLOR/NUMBER_OF_ITEMS",
              "SIZE/MATERIAL",
              "SIZE/NUMBER_OF_ITEMS",
              "SIZE/UNIT_COUNT",
              "SIZE_NAME",
              "SIZE_NAME/COLOR_NAME",
              "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS",
              "SIZE_NAME/ITEM_DISPLAY_WEIGHT",
              "SIZE_NAME/MATERIAL_TYPE",
              "SIZE_NAME/NUMBER_OF_ITEMS",
              "SIZE_NAME/PART_NUMBER",
              "SIZE_NAME/PATTERN_NAME",
              "SIZE_NAME/STYLE_NAME",
              "SIZE_NAME/UNIT_COUNT",
              "STYLE_NAME",
              "STYLE_NAME/COLOR_NAME",
              "STYLE_NAME/COLOR_NAME/SIZE_NAME",
              "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
              "STYLE_NAME/PATTERN_NAME",
              "STYLE_NAME/SIZE_NAME",
              "TEAM_NAME",
              "TEAM_NAME/SIZE_NAME",
              "VOLTAGE",
              "WATTAGE"
            ],
            "type": "string",
            "title": "Variation Theme Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "Size/Color"
            ],
            "enumNames": [
              "COLOR",
              "COLOR/MATERIAL",
              "COLOR/NUMBER_OF_ITEMS",
              "COLOR/SIZE",
              "COLOR/WATTAGE",
              "COLOR_NAME",
              "COLOR_NAME/ITEM_DISPLAY_WEIGHT",
              "COLOR_NAME/MATERIAL_TYPE",
              "COLOR_NAME/NUMBER_OF_ITEMS",
              "COLOR_NAME/SIZE_NAME",
              "COLOR_NAME/SIZE_NAME/STYLE_NAME",
              "COLOR_NAME/STYLE_NAME",
              "COLOR_NAME/WATTAGE",
              "CUSTOMER_PACKAGE_TYPE",
              "FLAVOR/SIZE",
              "FLAVOR_NAME",
              "ITEM_DISPLAY_WEIGHT",
              "ITEM_DISPLAY_WEIGHT/COLOR_NAME",
              "ITEM_DISPLAY_WEIGHT/MATERIAL_TYPE",
              "ITEM_DISPLAY_WEIGHT/SIZE_NAME",
              "ITEM_PACKAGE_QUANTITY",
              "ITEM_PACKAGE_QUANTITY/COLOR_NAME",
              "ITEM_PACKAGE_QUANTITY/SIZE_NAME",
              "ITEM_PACKAGE_QUANTITY/STYLE_NAME",
              "ITEM_WEIGHT",
              "MATERIAL/COLOR",
              "MATERIAL/SIZE",
              "MATERIAL_TYPE",
              "MATERIAL_TYPE/COLOR_NAME",
              "MATERIAL_TYPE/ITEM_DISPLAY_WEIGHT",
              "MATERIAL_TYPE/SIZE_NAME",
              "MODEL",
              "MODEL/SIZE_NAME",
              "MODEL_NAME",
              "MODEL_NAME/TEAM_NAME",
              "MODEL_NUMBER/SIZE",
              "NUMBER_OF_ITEMS",
              "PATTERN",
              "PATTERN_NAME",
              "PATTERN_NAME/SIZE_NAME",
              "SIZE",
              "SIZE/COLOR",
              "SIZE/COLOR/NUMBER_OF_ITEMS",
              "SIZE/MATERIAL",
              "SIZE/NUMBER_OF_ITEMS",
              "SIZE/UNIT_COUNT",
              "SIZE_NAME",
              "SIZE_NAME/COLOR_NAME",
              "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS",
              "SIZE_NAME/ITEM_DISPLAY_WEIGHT",
              "SIZE_NAME/MATERIAL_TYPE",
              "SIZE_NAME/NUMBER_OF_ITEMS",
              "SIZE_NAME/PART_NUMBER",
              "SIZE_NAME/PATTERN_NAME",
              "SIZE_NAME/STYLE_NAME",
              "SIZE_NAME/UNIT_COUNT",
              "STYLE_NAME",
              "STYLE_NAME/COLOR_NAME",
              "STYLE_NAME/COLOR_NAME/SIZE_NAME",
              "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
              "STYLE_NAME/PATTERN_NAME",
              "STYLE_NAME/SIZE_NAME",
              "TEAM_NAME",
              "TEAM_NAME/SIZE_NAME",
              "VOLTAGE",
              "WATTAGE"
            ],
            "$lifecycle": {
              "enumDeprecated": [
                "COLOR/MATERIAL",
                "COLOR/WATTAGE",
                "COLOR_NAME",
                "COLOR_NAME/ITEM_DISPLAY_WEIGHT",
                "COLOR_NAME/MATERIAL_TYPE",
                "COLOR_NAME/NUMBER_OF_ITEMS",
                "COLOR_NAME/SIZE_NAME",
                "COLOR_NAME/SIZE_NAME/STYLE_NAME",
                "COLOR_NAME/STYLE_NAME",
                "COLOR_NAME/WATTAGE",
                "CUSTOMER_PACKAGE_TYPE",
                "FLAVOR/SIZE",
                "FLAVOR_NAME",
                "ITEM_DISPLAY_WEIGHT",
                "ITEM_DISPLAY_WEIGHT/COLOR_NAME",
                "ITEM_DISPLAY_WEIGHT/MATERIAL_TYPE",
                "ITEM_DISPLAY_WEIGHT/SIZE_NAME",
                "ITEM_PACKAGE_QUANTITY",
                "ITEM_PACKAGE_QUANTITY/COLOR_NAME",
                "ITEM_PACKAGE_QUANTITY/SIZE_NAME",
                "ITEM_PACKAGE_QUANTITY/STYLE_NAME",
                "ITEM_WEIGHT",
                "MATERIAL/COLOR",
                "MATERIAL/SIZE",
                "MATERIAL_TYPE",
                "MATERIAL_TYPE/COLOR_NAME",
                "MATERIAL_TYPE/ITEM_DISPLAY_WEIGHT",
                "MATERIAL_TYPE/SIZE_NAME",
                "MODEL",
                "MODEL/SIZE_NAME",
                "MODEL_NAME",
                "MODEL_NAME/TEAM_NAME",
                "MODEL_NUMBER/SIZE",
                "PATTERN",
                "PATTERN_NAME",
                "PATTERN_NAME/SIZE_NAME",
                "SIZE/COLOR",
                "SIZE/MATERIAL",
                "SIZE_NAME",
                "SIZE_NAME/COLOR_NAME",
                "SIZE_NAME/COLOR_NAME/NUMBER_OF_ITEMS",
                "SIZE_NAME/ITEM_DISPLAY_WEIGHT",
                "SIZE_NAME/MATERIAL_TYPE",
                "SIZE_NAME/NUMBER_OF_ITEMS",
                "SIZE_NAME/PART_NUMBER",
                "SIZE_NAME/PATTERN_NAME",
                "SIZE_NAME/STYLE_NAME",
                "SIZE_NAME/UNIT_COUNT",
                "STYLE_NAME",
                "STYLE_NAME/COLOR_NAME",
                "STYLE_NAME/COLOR_NAME/SIZE_NAME",
                "STYLE_NAME/MODEL/NUMBER_OF_ITEMS/PART_NUMBER",
                "STYLE_NAME/PATTERN_NAME",
                "STYLE_NAME/SIZE_NAME",
                "TEAM_NAME",
                "TEAM_NAME/SIZE_NAME",
                "VOLTAGE",
                "WATTAGE"
              ]
            },
            "description": "Specify the variation theme that the product will use. The theme's attributes must be populated for all items in the grouping."
          }
        },
        "additionalProperties": false
      },
      "title": "Variation Theme",
      "examples": [
        "Size/Color"
      ],
      "maxItems": 1,
      "minItems": 1,
      "description": "Specify the variation theme that the product will use. The theme's attributes must be populated for all items in the grouping."
    },
    "compliance_media": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "content_language",
          "content_type",
          "source_location"
        ],
        "properties": {
          "content_type": {
            "enum": [
              "application_guide",
              "certificate_of_analysis",
              "certificate_of_compliance",
              "compatibility_guide",
              "emergency_use_authorization",
              "emergency_use_authorization_amendment",
              "installation_manual",
              "instructions_for_use",
              "patient_fact_sheet",
              "provider_fact_sheet",
              "safety_data_sheet",
              "safety_information",
              "specification_sheet",
              "troubleshooting_guide",
              "user_guide",
              "user_manual",
              "warranty"
            ],
            "type": "string",
            "title": "Compliance Media Content Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "Safety Data Sheet"
            ],
            "enumNames": [
              "Application Guide",
              "Certificate of Analysis",
              "Certificate of Compliance",
              "Compatibility Guide",
              "Emergency Use Authorization",
              "Emergency Use Authorization Amendment",
              "Installation Manual",
              "Instructions for Use",
              "Patient Fact Sheet",
              "Provider Fact Sheet",
              "Safety Data Sheet",
              "Safety Information",
              "Specification Sheet",
              "Troubleshooting Guide",
              "User Guide",
              "User Manual",
              "Warranty"
            ],
            "description": "Please enter the content type of the compliance document."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "source_location": {
            "type": "string",
            "title": "Compliance Media Source Location",
            "hidden": false,
            "editable": true,
            "examples": [
              "http://example.eg/sds_1.pdf"
            ],
            "description": "Provide the source location of the compliance media."
          },
          "content_language": {
            "enum": [
              "ar_AE",
              "ar_BH",
              "ar_DZ",
              "ar_EG",
              "ar_IQ",
              "ar_JO",
              "ar_KW",
              "ar_LB",
              "ar_LY",
              "ar_MA",
              "ar_OM",
              "ar_QA",
              "ar_SA",
              "ar_SD",
              "ar_SY",
              "ar_TN",
              "ar_YE",
              "az_AZ",
              "be_BY",
              "bg_BG",
              "bn_IN",
              "bs_BA",
              "ca_AD",
              "ca_ES",
              "cs_CZ",
              "da_DK",
              "de_AT",
              "de_CH",
              "de_DE",
              "de_LU",
              "el_CY",
              "el_GR",
              "en_AE",
              "en_AU",
              "en_CA",
              "en_GB",
              "en_IE",
              "en_IN",
              "en_MT",
              "en_NG",
              "en_NZ",
              "en_PH",
              "en_SG",
              "en_US",
              "en_ZA",
              "es_AR",
              "es_BO",
              "es_CL",
              "es_CO",
              "es_CR",
              "es_DO",
              "es_EC",
              "es_ES",
              "es_GT",
              "es_HN",
              "es_MX",
              "es_NI",
              "es_PA",
              "es_PE",
              "es_PR",
              "es_PY",
              "es_SV",
              "es_US",
              "es_UY",
              "es_VE",
              "et_EE",
              "fi_FI",
              "fil",
              "fil_PH",
              "fr_BE",
              "fr_CA",
              "fr_CH",
              "fr_FR",
              "fr_LU",
              "ga_IE",
              "gu_IN",
              "he_IL",
              "hi_IN",
              "hr_HR",
              "hu_HU",
              "id_ID",
              "in_ID",
              "is_IS",
              "it_CH",
              "it_IT",
              "iw_IL",
              "ja_JP",
              "ka_GE",
              "kn_IN",
              "ko_KR",
              "lt_LT",
              "lv_LV",
              "mk_MK",
              "ml_IN",
              "mr_IN",
              "ms_MY",
              "mt_MT",
              "nb_NO",
              "nl_BE",
              "nl_NL",
              "no_NO",
              "pl_PL",
              "pt_BR",
              "pt_PT",
              "ro_RO",
              "ru_RU",
              "sk_SK",
              "sl_SI",
              "sq_AL",
              "sr_BA",
              "sr_CS",
              "sr_ME",
              "sr_RS",
              "sv_SE",
              "ta_IN",
              "te_IN",
              "th_TH",
              "tr_TR",
              "uk_UA",
              "vi_VN",
              "zh_CN",
              "zh_HK",
              "zh_SG",
              "zh_TW"
            ],
            "type": "string",
            "title": "Compliance Media Language",
            "hidden": false,
            "editable": true,
            "examples": [
              "en_US"
            ],
            "enumNames": [
              "ar_AE",
              "ar_BH",
              "ar_DZ",
              "ar_EG",
              "ar_IQ",
              "ar_JO",
              "ar_KW",
              "ar_LB",
              "ar_LY",
              "ar_MA",
              "ar_OM",
              "ar_QA",
              "ar_SA",
              "ar_SD",
              "ar_SY",
              "ar_TN",
              "ar_YE",
              "az_AZ",
              "be_BY",
              "bg_BG",
              "bn_IN",
              "bs_BA",
              "ca_AD",
              "ca_ES",
              "cs_CZ",
              "da_DK",
              "de_AT",
              "de_CH",
              "de_DE",
              "de_LU",
              "el_CY",
              "el_GR",
              "en_AE",
              "en_AU",
              "en_CA",
              "en_GB",
              "en_IE",
              "en_IN",
              "en_MT",
              "en_NG",
              "en_NZ",
              "en_PH",
              "en_SG",
              "en_US",
              "en_ZA",
              "es_AR",
              "es_BO",
              "es_CL",
              "es_CO",
              "es_CR",
              "es_DO",
              "es_EC",
              "es_ES",
              "es_GT",
              "es_HN",
              "es_MX",
              "es_NI",
              "es_PA",
              "es_PE",
              "es_PR",
              "es_PY",
              "es_SV",
              "es_US",
              "es_UY",
              "es_VE",
              "et_EE",
              "fi_FI",
              "fil",
              "fil_PH",
              "fr_BE",
              "fr_CA",
              "fr_CH",
              "fr_FR",
              "fr_LU",
              "ga_IE",
              "gu_IN",
              "he_IL",
              "hi_IN",
              "hr_HR",
              "hu_HU",
              "id_ID",
              "in_ID",
              "is_IS",
              "it_CH",
              "it_IT",
              "iw_IL",
              "ja_JP",
              "ka_GE",
              "kn_IN",
              "ko_KR",
              "lt_LT",
              "lv_LV",
              "mk_MK",
              "ml_IN",
              "mr_IN",
              "ms_MY",
              "mt_MT",
              "nb_NO",
              "nl_BE",
              "nl_NL",
              "no_NO",
              "pl_PL",
              "pt_BR",
              "pt_PT",
              "ro_RO",
              "ru_RU",
              "sk_SK",
              "sl_SI",
              "sq_AL",
              "sr_BA",
              "sr_CS",
              "sr_ME",
              "sr_RS",
              "sv_SE",
              "ta_IN",
              "te_IN",
              "th_TH",
              "tr_TR",
              "uk_UA",
              "vi_VN",
              "zh_CN",
              "zh_HK",
              "zh_SG",
              "zh_TW"
            ],
            "description": "Provide the language used for the content of the compliance media."
          }
        },
        "additionalProperties": false
      },
      "title": "Compliance Media",
      "examples": [
        "Installation Manual"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "content_type",
        "content_language"
      ],
      "description": "Provide information on the product documents you want to display on the product detail page to comply with the General Product Safety Regulation (GPSR). Alternatively, you can upload images under the PS01-PS06 variants in the Image Manager.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "manufacture_year": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Manufacture Year",
            "hidden": false,
            "maximum": 4000,
            "minimum": 1900,
            "editable": true,
            "examples": [
              "2023"
            ],
            "description": "Provide the year the item was manufactured."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Manufacture Year",
      "examples": [
        "2023"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the year the item was manufactured.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "product_tax_code": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Product Tax Code",
            "hidden": false,
            "editable": true,
            "examples": [
              "A_GEN_NOTAX"
            ],
            "maxLength": 949,
            "description": "Enter the product tax code supplied to you by Amazon.com"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Product Tax Code",
      "examples": [
        "A_GEN_NOTAX"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Enter the product tax code supplied to you by Amazon.com",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "care_instructions": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Dishwasher Safe",
                  "Hand Wash",
                  "Microwave Safe"
                ],
                "type": "string",
                "enumNames": [
                  "Dishwasher Safe",
                  "Hand Wash",
                  "Microwave Safe"
                ]
              }
            ],
            "title": "Care Instructions",
            "hidden": false,
            "editable": true,
            "examples": [
              "Dishwasher Safe"
            ],
            "maxLength": 500,
            "description": "Provide instructions related to how to care for the item"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Product Care Instructions",
      "examples": [
        "Hand Wash"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide instructions related to how to care for the item",
      "maxUniqueItems": 2,
      "minUniqueItems": 1
    },
    "country_of_origin": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "AF",
              "AX",
              "AL",
              "DZ",
              "AS",
              "AD",
              "AO",
              "AI",
              "AQ",
              "AG",
              "AR",
              "AM",
              "AW",
              "AC",
              "AU",
              "AT",
              "AZ",
              "BH",
              "BD",
              "BB",
              "BY",
              "BE",
              "BZ",
              "BJ",
              "BM",
              "BT",
              "BO",
              "BQ",
              "BA",
              "BW",
              "BV",
              "BR",
              "IO",
              "VG",
              "BN",
              "BG",
              "BF",
              "BI",
              "KH",
              "CM",
              "CA",
              "IC",
              "CV",
              "KY",
              "CF",
              "TD",
              "CL",
              "CN",
              "CX",
              "CC",
              "CO",
              "KM",
              "CG",
              "CK",
              "CR",
              "HR",
              "CU",
              "CW",
              "CY",
              "CZ",
              "KP",
              "DK",
              "DJ",
              "DM",
              "DO",
              "TP",
              "EC",
              "EG",
              "SV",
              "GQ",
              "ER",
              "EE",
              "ET",
              "FK",
              "FO",
              "FM",
              "FJ",
              "FI",
              "FR",
              "GF",
              "PF",
              "TF",
              "GA",
              "GE",
              "DE",
              "GH",
              "GI",
              "GB",
              "GR",
              "GL",
              "GD",
              "GP",
              "GU",
              "GT",
              "GG",
              "GN",
              "GW",
              "GY",
              "HT",
              "HM",
              "VA",
              "HN",
              "HK",
              "HU",
              "IS",
              "IN",
              "ID",
              "IR",
              "IE",
              "IQ",
              "IM",
              "IL",
              "IT",
              "CI",
              "JM",
              "JP",
              "JE",
              "JO",
              "KZ",
              "KE",
              "KI",
              "KW",
              "KG",
              "LA",
              "LV",
              "LB",
              "LS",
              "LR",
              "LY",
              "LI",
              "LT",
              "LU",
              "MO",
              "MK",
              "MG",
              "MW",
              "MY",
              "MV",
              "ML",
              "MT",
              "MH",
              "MQ",
              "MR",
              "MU",
              "YT",
              "MX",
              "MC",
              "MN",
              "ME",
              "MS",
              "MA",
              "MZ",
              "MM",
              "NA",
              "NR",
              "NP",
              "NL",
              "AN",
              "NC",
              "NZ",
              "NI",
              "NE",
              "NG",
              "NU",
              "NF",
              "MP",
              "NO",
              "OM",
              "PK",
              "PW",
              "PS",
              "PA",
              "PG",
              "PY",
              "PE",
              "PH",
              "PN",
              "PL",
              "PT",
              "PR",
              "QA",
              "KR",
              "MD",
              "RE",
              "RO",
              "RU",
              "RW",
              "BL",
              "SH",
              "KN",
              "LC",
              "MF",
              "PM",
              "VC",
              "WS",
              "SM",
              "ST",
              "SA",
              "SN",
              "RS",
              "CS",
              "SC",
              "SL",
              "SG",
              "SX",
              "SK",
              "SI",
              "SB",
              "SO",
              "ZA",
              "GS",
              "SS",
              "ES",
              "LK",
              "SD",
              "SR",
              "SJ",
              "SZ",
              "SE",
              "CH",
              "SY",
              "TW",
              "TJ",
              "TH",
              "BS",
              "CD",
              "GM",
              "TL",
              "TG",
              "TK",
              "TO",
              "TT",
              "TA",
              "TN",
              "TR",
              "TM",
              "TC",
              "TV",
              "VI",
              "UG",
              "UA",
              "AE",
              "UK",
              "TZ",
              "US",
              "UM",
              "unknown",
              "UY",
              "UZ",
              "VU",
              "VE",
              "VN",
              "WF",
              "WD",
              "EH",
              "WZ",
              "XB",
              "XC",
              "XE",
              "XK",
              "XM",
              "XN",
              "XY",
              "YE",
              "YU",
              "ZR",
              "ZM",
              "ZW"
            ],
            "type": "string",
            "title": "Country of Origin",
            "hidden": false,
            "editable": false,
            "examples": [
              "China"
            ],
            "enumNames": [
              "Afghanistan",
              "Aland Islands",
              "Albania",
              "Algeria",
              "American Samoa",
              "Andorra",
              "Angola",
              "Anguilla",
              "Antarctica",
              "Antigua and Barbuda",
              "Argentina",
              "Armenia",
              "Aruba",
              "Ascension Island",
              "Australia",
              "Austria",
              "Azerbaijan",
              "Bahrain",
              "Bangladesh",
              "Barbados",
              "Belarus",
              "Belgium",
              "Belize",
              "Benin",
              "Bermuda",
              "Bhutan",
              "Bolivia",
              "Bonaire, Saint Eustatius and Saba",
              "Bosnia and Herzegovina",
              "Botswana",
              "Bouvet Island",
              "Brazil",
              "British Indian Ocean Territory",
              "British Virgin Islands",
              "Brunei Darussalam",
              "Bulgaria",
              "Burkina Faso",
              "Burundi",
              "Cambodia",
              "Cameroon",
              "Canada",
              "Canary Islands",
              "Cape Verde",
              "Cayman Islands",
              "Central African Republic",
              "Chad",
              "Chile",
              "China",
              "Christmas Island",
              "Cocos (Keeling) Islands",
              "Colombia",
              "Comoros",
              "Congo",
              "Cook Islands",
              "Costa Rica",
              "Croatia",
              "Cuba",
              "Curaçao",
              "Cyprus",
              "Czech Republic",
              "Democratic People's Republic of Korea",
              "Denmark",
              "Djibouti",
              "Dominica",
              "Dominican Republic",
              "East Timor",
              "Ecuador",
              "Egypt",
              "El Salvador",
              "Equatorial Guinea",
              "Eritrea",
              "Estonia",
              "Ethiopia",
              "Falkland Islands (Malvinas)",
              "Faroe Islands",
              "Federated States of Micronesia",
              "Fiji",
              "Finland",
              "France",
              "French Guiana",
              "French Polynesia",
              "French Southern Territories",
              "Gabon",
              "Georgia",
              "Germany",
              "Ghana",
              "Gibraltar",
              "Great Britain",
              "Greece",
              "Greenland",
              "Grenada",
              "Guadeloupe",
              "Guam",
              "Guatemala",
              "Guernsey",
              "Guinea",
              "Guinea-Bissau",
              "Guyana",
              "Haiti",
              "Heard Island and the McDonald Islands",
              "Holy See",
              "Honduras",
              "Hong Kong",
              "Hungary",
              "Iceland",
              "India",
              "Indonesia",
              "Iran",
              "Ireland",
              "Islamic Republic of Iraq",
              "Isle of Man",
              "Israel",
              "Italy",
              "Ivory Coast",
              "Jamaica",
              "Japan",
              "Jersey",
              "Jordan",
              "Kazakhstan",
              "Kenya",
              "Kiribati",
              "Kuwait",
              "Kyrgyzstan",
              "Lao People's Democratic Republic",
              "Latvia",
              "Lebanon",
              "Lesotho",
              "Liberia",
              "Libya",
              "Liechtenstein",
              "Lithuania",
              "Luxembourg",
              "Macao",
              "Macedonia",
              "Madagascar",
              "Malawi",
              "Malaysia",
              "Maldives",
              "Mali",
              "Malta",
              "Marshall Islands",
              "Martinique",
              "Mauritania",
              "Mauritius",
              "Mayotte",
              "Mexico",
              "Monaco",
              "Mongolia",
              "Montenegro",
              "Montserrat",
              "Morocco",
              "Mozambique",
              "Myanmar",
              "Namibia",
              "Nauru",
              "Nepal",
              "Netherlands",
              "Netherlands Antilles",
              "New Caledonia",
              "New Zealand",
              "Nicaragua",
              "Niger",
              "Nigeria",
              "Niue",
              "Norfolk Island",
              "Northern Mariana Islands",
              "Norway",
              "Oman",
              "Pakistan",
              "Palau",
              "Palestinian Territories",
              "Panama",
              "Papua New Guinea",
              "Paraguay",
              "Peru",
              "Philippines",
              "Pitcairn",
              "Poland",
              "Portugal",
              "Puerto Rico",
              "Qatar",
              "Republic of Korea",
              "Republic of Moldova",
              "Reunion",
              "Romania",
              "Russian Federation",
              "Rwanda",
              "Saint Barthelemy",
              "Saint Helena, Ascension and Tristan da Cunha",
              "Saint Kitts and Nevis",
              "Saint Lucia",
              "Saint Martin",
              "Saint Pierre and Miquelon",
              "Saint Vincent and the Grenadines",
              "Samoa",
              "San Marino",
              "Sao Tome and Principe",
              "Saudi Arabia",
              "Senegal",
              "Serbia",
              "Serbia and Montenegro",
              "Seychelles",
              "Sierra Leone",
              "Singapore",
              "Sint Maarten",
              "Slovakia",
              "Slovenia",
              "Solomon Islands",
              "Somalia",
              "South Africa",
              "South Georgia and the South Sandwich Islands",
              "South Sudan",
              "Spain",
              "Sri Lanka",
              "Sudan",
              "Suriname",
              "Svalbard and Jan Mayen",
              "Swaziland",
              "Sweden",
              "Switzerland",
              "Syria",
              "Taiwan",
              "Tajikistan",
              "Thailand",
              "The Bahamas",
              "The Democratic Republic of the Congo",
              "The Gambia",
              "Timor-Leste",
              "Togo",
              "Tokelau",
              "Tonga",
              "Trinidad and Tobago",
              "Tristan da Cunha",
              "Tunisia",
              "Turkey",
              "Turkmenistan",
              "Turks and Caicos Islands",
              "Tuvalu",
              "U.S. Virgin Islands",
              "Uganda",
              "Ukraine",
              "United Arab Emirates",
              "United Kingdom",
              "United Republic of Tanzania",
              "United States",
              "United States Minor Outlying Islands",
              "Unknown",
              "Uruguay",
              "Uzbekistan",
              "Vanuatu",
              "Venezuela",
              "Vietnam",
              "Wallis and Futuna",
              "WD",
              "Western Sahara",
              "WZ",
              "XB",
              "XC",
              "XE",
              "XK",
              "XM",
              "XN",
              "XY",
              "Yemen",
              "Yugoslavia",
              "Zaire",
              "Zambia",
              "Zimbabwe"
            ],
            "description": "Select the product's country of origin"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Country of Publication",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The country in which the product was published.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_type_keyword": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Item Type Keyword",
            "hidden": false,
            "editable": false,
            "examples": [
              "Food mills"
            ],
            "maxLength": 20090,
            "description": "Item type keywords are used to place new ASINs in the appropriate place(s) within the graph. Select the most specific accurate term for optimal placement."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Type Keyword",
      "examples": [
        "Food mills"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "What is the item that you are selling?",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "pesticide_marking": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "marking_type"
        ],
        "properties": {
          "marking_type": {
            "enum": [
              "epa_establishment_number",
              "epa_registration_number"
            ],
            "type": "string",
            "title": "Pesticide Marking",
            "hidden": false,
            "editable": true,
            "examples": [
              "EPA Establishment Number"
            ],
            "enumNames": [
              "EPA Establishment Number",
              "EPA Registration Number"
            ],
            "description": "Provide any pesticide marking on the item or packaging."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "registration_status": {
            "enum": [
              "fifra_registration_required",
              "fifra_not_considered_pesticide",
              "fifra_registration_exempt"
            ],
            "type": "string",
            "title": "Pesticide Registration Status",
            "hidden": false,
            "editable": true,
            "examples": [
              "Product is not a pesticide or pesticide device, as defined under the U.S. Federal Insecticide, Fungicide, and Rodenticide Act."
            ],
            "enumNames": [
              "This product is a pesticide or pesticide device, as defined under the U.S. Federal Insecticide, Fungicide, and Rodenticide Act",
              "This product is not a pesticide or pesticide device, as defined under the U.S. Federal Insecticide, Fungicide, and Rodenticide Act.",
              "This product qualifies for an exemption from registration under the U.S. Federal Insecticide, Fungicide, and Rodenticide Act."
            ],
            "description": "Provide a status whether the item requires registration and an associated registration number."
          },
          "certification_number": {
            "type": "string",
            "title": "Pesticide Certification Number",
            "hidden": false,
            "editable": true,
            "examples": [
              "138263"
            ],
            "maxLength": 300,
            "description": "Provide any pesticide certification number which corresponds with the marking type"
          }
        },
        "additionalProperties": false
      },
      "title": "Pesticide Marking",
      "examples": [
        "EPA Establishment Number"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "marking_type"
      ],
      "description": "Provide any pesticide marking on the item or packaging.",
      "maxUniqueItems": 3,
      "minUniqueItems": 1
    },
    "purchasable_offer": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "end_at": {
            "type": "object",
            "title": "Purchasable Offer End At",
            "required": [],
            "properties": {
              "value": {
                "type": "string",
                "oneOf": [
                  {
                    "type": "string",
                    "format": "date"
                  },
                  {
                    "type": "string",
                    "format": "date-time"
                  }
                ],
                "title": "Stop Selling Date",
                "hidden": false,
                "editable": true,
                "examples": [
                  "2017-07-01"
                ],
                "description": "Your price end date"
              }
            },
            "description": "The attribute indicates the Purchasable Offer End At of the product",
            "additionalProperties": false
          },
          "audience": {
            "enum": [
              "ALL"
            ],
            "type": "string",
            "title": "Audience",
            "hidden": true,
            "editable": false,
            "examples": [
              "B2B"
            ],
            "enumNames": [
              "Sell on Amazon"
            ],
            "description": "Provide the intended buyer segment or program that this purchasable offer is applicable to."
          },
          "currency": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "USD"
                ],
                "type": "string",
                "enumNames": [
                  "USD"
                ]
              }
            ],
            "title": "Currency",
            "hidden": true,
            "default": "USD",
            "editable": false,
            "examples": [
              "USD"
            ],
            "description": "Select the corresponding currency"
          },
          "start_at": {
            "type": "object",
            "title": "Purchasable Offer Start At",
            "required": [],
            "properties": {
              "value": {
                "type": "string",
                "oneOf": [
                  {
                    "type": "string",
                    "format": "date"
                  },
                  {
                    "type": "string",
                    "format": "date-time"
                  }
                ],
                "title": "Offering Release Date",
                "hidden": false,
                "editable": true,
                "examples": [
                  "2017-06-30"
                ],
                "description": "Your price start date"
              }
            },
            "description": "The attribute indicates the Purchasable Offer Start At of the product",
            "additionalProperties": false
          },
          "map_price": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [],
                    "properties": {
                      "value_with_tax": {
                        "type": "number",
                        "title": "Minimum Advertised Price",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "259.99"
                        ],
                        "description": "Provide the minimum advertised price"
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Purchasable Offer Map Price Schedule",
                  "minItems": 1,
                  "description": "The attribute indicates the Purchasable Offer Map Price Schedule of the product"
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Offer Map Price",
            "minItems": 1,
            "description": "The attribute indicates the Purchasable Offer Map Price of the product"
          },
          "our_price": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "schedule"
              ],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [
                      "value_with_tax"
                    ],
                    "properties": {
                      "value_with_tax": {
                        "type": "number",
                        "title": "Your Price",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "9.00"
                        ],
                        "description": "Provide base price of the item at which it is being offered to the intended buyer segment"
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Purchasable Offer Our Price Schedule",
                  "minItems": 1,
                  "description": "The attribute indicates the Purchasable Offer Our Price Schedule of the product"
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Offer Our Price",
            "minItems": 1,
            "description": "The attribute indicates the Purchasable Offer Our Price of the product"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "discounted_price": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "schedule"
              ],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [
                      "end_at",
                      "start_at",
                      "value_with_tax"
                    ],
                    "properties": {
                      "end_at": {
                        "type": "string",
                        "oneOf": [
                          {
                            "type": "string",
                            "format": "date"
                          },
                          {
                            "type": "string",
                            "format": "date-time"
                          }
                        ],
                        "title": "Sale End Date",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "2017-07-01"
                        ],
                        "description": "The last date that the sale price will override the item's standard price; the product's standard price will be displayed after 0:00AM of Sale End Date."
                      },
                      "start_at": {
                        "type": "string",
                        "oneOf": [
                          {
                            "type": "string",
                            "format": "date"
                          },
                          {
                            "type": "string",
                            "format": "date-time"
                          }
                        ],
                        "title": "Sale Start Date",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "2017-06-30"
                        ],
                        "description": "The date that the sale price will begin to override the product's standard price; the sale price will be displayed after 0:00AM of Sale From Date."
                      },
                      "value_with_tax": {
                        "type": "number",
                        "title": "Sale Price",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "219.99"
                        ],
                        "description": "The price at which you offer the product for sale."
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Purchasable Offer Discounted Price Schedule",
                  "minItems": 1,
                  "description": "The attribute indicates the Purchasable Offer Discounted Price Schedule of the product"
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Offer Discounted Price",
            "minItems": 1,
            "description": "The attribute indicates the Purchasable Offer Discounted Price of the product"
          },
          "quantity_discount_plan": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [
                "schedule"
              ],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [
                      "discount_type",
                      "levels"
                    ],
                    "properties": {
                      "levels": {
                        "type": "array",
                        "items": {
                          "type": "object",
                          "required": [
                            "lower_bound",
                            "value"
                          ],
                          "properties": {
                            "value": {
                              "type": "number",
                              "title": "Quantity Price (Fixed Price/Percentage Discount)",
                              "hidden": false,
                              "minimum": 0,
                              "editable": true,
                              "examples": [
                                "10, 20"
                              ],
                              "description": "Provide the quantity price for each quantity threshold or the discount percentage offered on the business price for each quantity threshold."
                            },
                            "lower_bound": {
                              "type": "integer",
                              "title": "Quantity Threshold (Lower Bound)",
                              "hidden": false,
                              "minimum": 0,
                              "editable": true,
                              "examples": [
                                "5, 10"
                              ],
                              "description": "Provide the minimum purchase quantity necessary to receive the discount. It will apply to all units if the quantity threshold is met."
                            }
                          },
                          "additionalProperties": false
                        },
                        "title": "Levels",
                        "examples": [
                          "Quantity Discount Plan Schedule Levels"
                        ],
                        "maxItems": 5,
                        "minItems": 1,
                        "description": "Quantity Discount Plan Schedule Levels"
                      },
                      "discount_type": {
                        "enum": [
                          "fixed",
                          "percent"
                        ],
                        "type": "string",
                        "title": "Quantity Price Type",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "Fixed, Percent"
                        ],
                        "enumNames": [
                          "Fixed",
                          "Percent"
                        ],
                        "description": "Provide whether the quantity price type is fixed, a price set in local currency for each quantity threshold, or a percentage of business price"
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Schedule",
                  "examples": [
                    "Quantity price start date: 06/30/2024; Quantity price end date: 07/01/2024"
                  ],
                  "minItems": 1,
                  "description": "Provide the details, such as dates, pricing type that define your scheduled quantity discount plan."
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Business Offer Quantity Discount Plan",
            "examples": [
              "Schedule Quantity Price Type: Fixed; Schedule Levels Quantity Lower Bound: 5; Schedule Levels Quantity Price: 10"
            ],
            "maxItems": 0,
            "minItems": 1,
            "description": "Provide and define the quantity discount plan for your business price."
          },
          "maximum_seller_allowed_price": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [],
                    "properties": {
                      "value_with_tax": {
                        "type": "number",
                        "title": "Maximum Seller Allowed Price",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "259.99"
                        ],
                        "description": "Provide the maximum seller allowed price"
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Purchasable Offer Maximum Seller Allowed Price Schedule",
                  "minItems": 1,
                  "description": "The attribute indicates the Purchasable Offer Maximum Seller Allowed Price Schedule of the product"
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Offer Maximum Seller Allowed Price",
            "minItems": 1,
            "description": "The attribute indicates the Purchasable Offer Maximum Seller Allowed Price of the product"
          },
          "minimum_seller_allowed_price": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [],
              "properties": {
                "schedule": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "required": [],
                    "properties": {
                      "value_with_tax": {
                        "type": "number",
                        "title": "Minimum Seller Alllowed Price",
                        "hidden": false,
                        "editable": true,
                        "examples": [
                          "259.99"
                        ],
                        "description": "Provide the minimum seller allowed price"
                      }
                    },
                    "additionalProperties": false
                  },
                  "title": "Purchasable Offer Minimum Seller Allowed Price Schedule",
                  "minItems": 1,
                  "description": "The attribute indicates the Purchasable Offer Minimum Seller Allowed Price Schedule of the product"
                }
              },
              "additionalProperties": false
            },
            "title": "Purchasable Offer Minimum Seller Allowed Price",
            "minItems": 1,
            "description": "The attribute indicates the Purchasable Offer Minimum Seller Allowed Price of the product"
          },
          "automated_pricing_merchandising_rule_plan": {
            "type": "array",
            "items": {
              "type": "object",
              "required": [],
              "properties": {
                "merchandising_rule": {
                  "type": "object",
                  "required": [
                    "rule_id"
                  ],
                  "properties": {
                    "rule_id": {
                      "type": "string",
                      "title": "Pricing Rule",
                      "hidden": false,
                      "editable": true,
                      "examples": [
                        "Competitive Price Rule by Amazon"
                      ],
                      "description": "The pricing rule that will automate price on this offer"
                    }
                  },
                  "additionalProperties": false
                }
              },
              "additionalProperties": false
            },
            "minItems": 1
          }
        },
        "additionalProperties": false
      },
      "title": "Purchasable Offer",
      "examples": [
        "EUR"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "currency",
        "audience"
      ],
      "description": "The attribute indicates the Purchasable Offer of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "batteries_included": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Are batteries included?",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Select \"yes\" if batteries are contained in the product (e.g. batteries inside a pair of Bluetooth headphones) and/or included with the product (e.g. batteries packed separately with a camera), otherwise select \"no\""
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Batteries are Included",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Indicate if batteries are included with the product.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "batteries_required": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Are batteries required?",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Select \"yes\" if batteries are required to power the item (or if the item is a battery) or \"no\" if they are not. Please note that an internal rechargeable battery is also considered a battery"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Are Batteries Required",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Indicate if batteries are required.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "master_pack_weight": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "unit",
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "grams",
              "hundredths_pounds",
              "kilograms",
              "milligrams",
              "ounces",
              "pounds",
              "tons"
            ],
            "type": "string",
            "title": "Master Pack Weight Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Pounds"
            ],
            "enumNames": [
              "Grams",
              "Hundredths Pounds",
              "Kilograms",
              "Milligrams",
              "Ounces",
              "Pounds",
              "Tons"
            ],
            "description": "Provide the corresponding unit used to designate the weight of the master pack item."
          },
          "value": {
            "type": "number",
            "title": "Master Pack Weight",
            "hidden": false,
            "maximum": 10000,
            "minimum": 0,
            "editable": true,
            "examples": [
              "25.3"
            ],
            "maxLength": 16,
            "multipleOf": 1e-12,
            "description": "Provide the weight measurement of the master pack item."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Master Pack Weight",
      "examples": [
        "25.3 Pounds"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the weight measurement of the master pack item.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "max_order_quantity": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Maximum Order Quantity",
            "hidden": false,
            "minimum": 1,
            "editable": true,
            "examples": [
              "3"
            ],
            "description": "Max order quantity."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Max Order Quantity",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Max order quantity.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "ghs_chemical_h_code": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "EUH014",
              "EUH018",
              "EUH019",
              "EUH029",
              "EUH031",
              "EUH032",
              "EUH044",
              "EUH066",
              "EUH070",
              "EUH071",
              "EUH201",
              "EUH201A",
              "EUH202",
              "EUH203",
              "EUH204",
              "EUH205",
              "EUH206",
              "EUH207",
              "EUH208",
              "EUH209",
              "EUH209A",
              "EUH210",
              "EUH211",
              "EUH212",
              "EUH380",
              "EUH381",
              "EUH401",
              "EUH430",
              "EUH431",
              "EUH440",
              "EUH441",
              "EUH450",
              "EUH451",
              "H200",
              "H201",
              "H202",
              "H203",
              "H204",
              "H205",
              "H220",
              "H221",
              "H222",
              "H223",
              "H224",
              "H225",
              "H226",
              "H228",
              "H229",
              "H230",
              "H231",
              "H240",
              "H241",
              "H242",
              "H250",
              "H251",
              "H252",
              "H260",
              "H261",
              "H270",
              "H271",
              "H272",
              "H280",
              "H281",
              "H290",
              "H300",
              "H301",
              "H302",
              "H304",
              "H310",
              "H311",
              "H312",
              "H314",
              "H315",
              "H317",
              "H318",
              "H319",
              "H330",
              "H331",
              "H332",
              "H334",
              "H335",
              "H336",
              "H340",
              "H341",
              "H350",
              "H350I",
              "H351",
              "H360",
              "H361",
              "H362",
              "H370",
              "H371",
              "H372",
              "H373",
              "H400",
              "H410",
              "H411",
              "H412",
              "H413",
              "H420"
            ],
            "type": "string",
            "title": "GHS Chemical H Code",
            "hidden": false,
            "editable": true,
            "examples": [
              "H200"
            ],
            "enumNames": [
              "EUH014",
              "EUH018",
              "EUH019",
              "EUH029",
              "EUH031",
              "EUH032",
              "EUH044",
              "EUH066",
              "EUH070",
              "EUH071",
              "EUH201",
              "EUH201A",
              "EUH202",
              "EUH203",
              "EUH204",
              "EUH205",
              "EUH206",
              "EUH207",
              "EUH208",
              "EUH209",
              "EUH209A",
              "EUH210",
              "EUH211",
              "EUH212",
              "EUH380",
              "EUH381",
              "EUH401",
              "EUH430",
              "EUH431",
              "EUH440",
              "EUH441",
              "EUH450",
              "EUH451",
              "H200",
              "H201",
              "H202",
              "H203",
              "H204",
              "H205",
              "H220",
              "H221",
              "H222",
              "H223",
              "H224",
              "H225",
              "H226",
              "H228",
              "H229",
              "H230",
              "H231",
              "H240",
              "H241",
              "H242",
              "H250",
              "H251",
              "H252",
              "H260",
              "H261",
              "H270",
              "H271",
              "H272",
              "H280",
              "H281",
              "H290",
              "H300",
              "H301",
              "H302",
              "H304",
              "H310",
              "H311",
              "H312",
              "H314",
              "H315",
              "H317",
              "H318",
              "H319",
              "H330",
              "H331",
              "H332",
              "H334",
              "H335",
              "H336",
              "H340",
              "H341",
              "H350",
              "H350I",
              "H351",
              "H360",
              "H361",
              "H362",
              "H370",
              "H371",
              "H372",
              "H373",
              "H400",
              "H410",
              "H411",
              "H412",
              "H413",
              "H420"
            ],
            "description": "Provide the GHS chemical hazard codes for the chemical substance/mixture in order to display warnings to customers."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "GHS Chemical H Code",
      "examples": [
        "H200"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "value"
      ],
      "description": "Provide the GHS chemical hazard codes for the chemical substance/mixture in order to display warnings to customers.",
      "maxUniqueItems": 100,
      "minUniqueItems": 1
    },
    "included_components": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Included Components",
            "hidden": false,
            "editable": true,
            "examples": [
              "Camera Body"
            ],
            "maxLength": 1000,
            "description": "Specify the items that are included with this product"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Included Components",
      "examples": [
        "Camera Body, Battery Pack"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Which components are included?",
      "maxUniqueItems": 79,
      "minUniqueItems": 1
    },
    "item_display_weight": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "unit",
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "grams",
              "hundredths_pounds",
              "kilograms",
              "milligrams",
              "ounces",
              "pounds",
              "tons"
            ],
            "type": "string",
            "title": "Item Display Weight Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Ounces, Pounds"
            ],
            "enumNames": [
              "Grams",
              "Hundredths Pounds",
              "Kilograms",
              "Milligrams",
              "Ounces",
              "Pounds",
              "Tons"
            ],
            "description": "Select the corresponding unit"
          },
          "value": {
            "type": "number",
            "title": "Item Display Weight",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "20.0, 50.0"
            ],
            "maxLength": 5000,
            "description": "Provide the item weight (numeric) if the product is a solid"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Display Weight",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the item weight if the product is a solid",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_package_weight": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "unit",
          "value"
        ],
        "properties": {
          "unit": {
            "enum": [
              "pounds"
            ],
            "type": "string",
            "title": "Package Weight Unit",
            "hidden": false,
            "editable": true,
            "examples": [
              "Pounds"
            ],
            "enumNames": [
              "Pounds"
            ],
            "description": "Select the unit of measure for Package Weight. If a value is provided for Package Weight, you must also enter the corresponding unit."
          },
          "value": {
            "type": "number",
            "title": "Package Weight",
            "hidden": false,
            "maximum": 1000000000,
            "minimum": 0,
            "editable": true,
            "examples": [
              "0.65"
            ],
            "description": "This attribute represents the weight of the item plus the packaging. If your item is shipped to the customer in multiple packages, enter the dimensions of the heaviest package",
            "exclusiveMinimum": 0
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Package Weight",
      "examples": [
        "14.89"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The weight in original package",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "product_description": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Product Description",
            "hidden": false,
            "editable": true,
            "examples": [
              "This summer, boots by Jette made from high quality suede leather are real gems. They visually highlight the craftsmanship and fine leather braid positioned at the top of the shaft"
            ],
            "description": "Provide a text description of the product. This information will appear in paragraph form on the detail page of your product. Include unique product features, product line details, and product specifications. Do not use all caps.",
            "maxUtf8ByteLength": 10000
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Product Description",
      "examples": [
        "This ham has been smoked for 12 hours..."
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "The description you provide should pertain to the product in general, not your particular item. There is a 2,000 character maximum.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "package_contains_sku": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "quantity",
          "sku"
        ],
        "properties": {
          "sku": {
            "type": "string",
            "title": "Package Contains SKU Identifier",
            "hidden": false,
            "editable": true,
            "examples": [
              "ABC123"
            ],
            "maxLength": 40,
            "minLength": 1,
            "description": "Provide the SKU identifier of each unit, case or pallet identified in Package Level.",
            "maxUtf8ByteLength": 40,
            "minUtf8ByteLength": 1
          },
          "quantity": {
            "type": "integer",
            "title": "Package Contains SKU Quantity",
            "hidden": false,
            "maximum": 250,
            "minimum": 1,
            "editable": true,
            "examples": [
              "1"
            ],
            "description": "Provide the quantity of each unit, case, or pallet identified in Package Level."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Package Contains SKU",
      "examples": [
        "SKU: ABC123, Quanitity: 1"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "sku"
      ],
      "description": "Provide the SKU and quantity of the child items contained in the next package level.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "customer_package_type": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Customer Package Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "Standard Packaging"
            ],
            "maxLength": 2176,
            "description": "Provide the products package type"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Customer Package Type",
      "examples": [
        "Standard Packaging"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide the products package type",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_package_quantity": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Item Package Quantity",
            "hidden": false,
            "minimum": 1,
            "editable": true,
            "examples": [
              "1"
            ],
            "description": "Provide the number of packages sold as part of a single item. An ASIN selling 5 boxes of paperclips with 100 paperclips per box would have item package quantity = '5'"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Package Quantity",
      "examples": [
        "3"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Quantity of the item for sale in one package",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "merchant_release_date": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "oneOf": [
              {
                "type": "string",
                "format": "date"
              },
              {
                "type": "string",
                "format": "date-time"
              }
            ],
            "title": "Merchant Release Date",
            "hidden": false,
            "editable": true,
            "examples": [
              "2017-07-20"
            ],
            "description": "Provide the merchant release date using YYYY-MM-DD format"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Offering Release Date",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the merchant release date using YYYY-MM-DD format",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "safety_data_sheet_url": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Safety Data Sheet (SDS or MSDS) URL",
            "hidden": false,
            "editable": true,
            "examples": [
              "www.safetysheetsRus.com/hazardous_substance/msds.pdf"
            ],
            "maxLength": 23397,
            "description": "Provide the web address for the Safety Data Sheet, containing essential safety information for potentially hazardous materials."
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Safety Data Sheet (SDS or MSDS) URL",
      "examples": [
        "www.safetysheetsRus.com/hazardous_substance/msds.pdf"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Provide the SDS/MSDS URL. Required for Hazardous material SDS/MSDS provides information such as physical data (flashpoint, pH, etc.), health concerns, storage, and transportation information for potentially dangerous substances.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "master_pack_dimensions": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "height",
          "length",
          "width"
        ],
        "properties": {
          "width": {
            "type": "object",
            "title": "Master Pack Width",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "angstrom",
                  "centimeters",
                  "decimeters",
                  "feet",
                  "hundredths_inches",
                  "inches",
                  "kilometers",
                  "meters",
                  "micrometer",
                  "miles",
                  "millimeters",
                  "mils",
                  "nanometer",
                  "picometer",
                  "yards"
                ],
                "type": "string",
                "title": "Master Pack Width Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Angstrom",
                  "Centimeters",
                  "Decimeters",
                  "Feet",
                  "Hundredths-Inches",
                  "Inches",
                  "Kilometers",
                  "Meters",
                  "Micron",
                  "Miles",
                  "Millimeters",
                  "Mils",
                  "Nanometer",
                  "Picometer",
                  "Yards"
                ],
                "description": "Provide the corresponding unit used to designate the width measurement of the master pack."
              },
              "value": {
                "type": "number",
                "title": "Master Pack Width",
                "hidden": false,
                "maximum": 10000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "32.4"
                ],
                "maxLength": 16,
                "multipleOf": 1e-12,
                "description": "Provide the width measurement of the master pack."
              }
            },
            "description": "Provide the width measurement of the master pack.",
            "additionalProperties": false
          },
          "height": {
            "type": "object",
            "title": "Master Pack Height",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "angstrom",
                  "centimeters",
                  "decimeters",
                  "feet",
                  "hundredths_inches",
                  "inches",
                  "kilometers",
                  "meters",
                  "micrometer",
                  "miles",
                  "millimeters",
                  "mils",
                  "nanometer",
                  "picometer",
                  "yards"
                ],
                "type": "string",
                "title": "Master Pack Height Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Angstrom",
                  "Centimeters",
                  "Decimeters",
                  "Feet",
                  "Hundredths-Inches",
                  "Inches",
                  "Kilometers",
                  "Meters",
                  "Micron",
                  "Miles",
                  "Millimeters",
                  "Mils",
                  "Nanometer",
                  "Picometer",
                  "Yards"
                ],
                "description": "Provide the corresponding unit used to designate the height measurement of the master pack."
              },
              "value": {
                "type": "number",
                "title": "Master Pack Height",
                "hidden": false,
                "maximum": 10000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "32.4"
                ],
                "maxLength": 16,
                "multipleOf": 1e-12,
                "description": "Provide the height measurement of the master pack."
              }
            },
            "description": "Provide the height measurement of the master pack.",
            "additionalProperties": false
          },
          "length": {
            "type": "object",
            "title": "Master Pack Length",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "angstrom",
                  "centimeters",
                  "decimeters",
                  "feet",
                  "hundredths_inches",
                  "inches",
                  "kilometers",
                  "meters",
                  "micrometer",
                  "miles",
                  "millimeters",
                  "mils",
                  "nanometer",
                  "picometer",
                  "yards"
                ],
                "type": "string",
                "title": "Master Pack Length Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Angstrom",
                  "Centimeters",
                  "Decimeters",
                  "Feet",
                  "Hundredths-Inches",
                  "Inches",
                  "Kilometers",
                  "Meters",
                  "Micron",
                  "Miles",
                  "Millimeters",
                  "Mils",
                  "Nanometer",
                  "Picometer",
                  "Yards"
                ],
                "description": "Provide the corresponding unit used to designate the length measurement of the master pack."
              },
              "value": {
                "type": "number",
                "title": "Master Pack Length",
                "hidden": false,
                "maximum": 10000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "32.4"
                ],
                "maxLength": 16,
                "multipleOf": 1e-12,
                "description": "Provide the length measurement of the master pack."
              }
            },
            "description": "Provide the length measurement of the master pack.",
            "additionalProperties": false
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Master Pack Dimensions",
      "examples": [
        "32.4 inches"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the width, height and depth measurements of the master pack.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "gpsr_safety_attestation": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "GPSR Safety Attestation",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Check “yes” if your product doesn’t have any warning and safety information, as it can be used safely and as intended without it."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "GPSR Safety Attestation",
      "examples": [
        "Yes"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Check “yes” if your product doesn’t have any warning and safety information, as it can be used safely and as intended without it.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "handmade_classification": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "hand_altered",
              "hand_designed",
              "handcrafted",
              "repurposed",
              "upcycled"
            ],
            "type": "string",
            "title": "Handmade Classification",
            "hidden": false,
            "editable": true,
            "examples": [
              "Hand-Altered"
            ],
            "enumNames": [
              "Hand-Altered",
              "Hand-Designed",
              "Handcrafted",
              "Repurposed",
              "Upcycled"
            ],
            "description": "Select the value that best describes how the product was produced"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Handmade Classification",
      "examples": [
        "Hand-Altered"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Select the value that best describes how the product was produced",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_package_dimensions": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "height",
          "length",
          "width"
        ],
        "properties": {
          "width": {
            "type": "object",
            "title": "Package Width",
            "examples": [
              "2"
            ],
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Package Width Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Select the unit of measure for Package Width. If a value is provided for Package Width, you must also enter the corresponding unit."
              },
              "value": {
                "type": "number",
                "title": "Item Package Width",
                "hidden": false,
                "maximum": 1000000000,
                "editable": true,
                "examples": [
                  "2"
                ],
                "description": "Provide the package width as a numeric value."
              }
            },
            "description": "Provide the package width",
            "additionalProperties": false
          },
          "height": {
            "type": "object",
            "title": "Package Height",
            "examples": [
              "2.7"
            ],
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Package Height Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Select the unit of measure for Package Height. If a value is provided for Package Height, you must also enter the corresponding unit."
              },
              "value": {
                "type": "number",
                "title": "Item Package Height",
                "hidden": false,
                "maximum": 1000000000,
                "editable": true,
                "examples": [
                  "2.7"
                ],
                "description": "Provide the package height as a numeric value."
              }
            },
            "description": "Provide the package height",
            "additionalProperties": false
          },
          "length": {
            "type": "object",
            "title": "Package Length",
            "examples": [
              "10"
            ],
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Package Length Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Select the unit of measure for Package Length. If a value is provided for Package Length, you must also enter the corresponding unit."
              },
              "value": {
                "type": "number",
                "title": "Item Package Length",
                "hidden": false,
                "maximum": 1000000000,
                "editable": true,
                "examples": [
                  "10"
                ],
                "description": "Provide the package length as a numeric value."
              }
            },
            "description": "Provide the package length",
            "additionalProperties": false
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Package Dimensions",
      "examples": [
        "10 x 2 x 2.7 inches"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the item's package dimensions",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "merchant_shipping_group": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Merchant Shipping Group",
            "hidden": false,
            "editable": true,
            "examples": [
              "Heavy Bulky Products, NCR Large Appliance Delivery"
            ],
            "maxLength": 100,
            "description": "The ship configuration group for an offer. The ship configuration group is created and managed by the seller through the ship setting UI."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Merchant Shipping Group",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The ship configuration group for an offer. The ship configuration group is created and managed by the seller through the ship setting UI.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "merchant_suggested_asin": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Merchant Suggested ASIN",
            "hidden": false,
            "editable": false,
            "examples": [
              "B007KQBXN0"
            ],
            "maxLength": 10,
            "minLength": 10,
            "description": "Provide an ASIN for your product if one exists. If a value is not provided, the system will attempt a match based on the External Product ID.",
            "maxUtf8ByteLength": 40
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Merchant Suggested ASIN",
      "examples": [
        "B007KQBXN0"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "value"
      ],
      "description": "Provide an ASIN for your product if one exists. If a value is not provided, the system will attempt a match based on the External Product ID.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "fulfillment_availability": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "fulfillment_channel_code"
        ],
        "properties": {
          "quantity": {
            "type": "integer",
            "title": "Quantity",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "152"
            ],
            "description": "Enter the quantity of the item you are making available for sale. This is your current inventory commitment (as a whole number)"
          },
          "restock_date": {
            "type": "string",
            "oneOf": [
              {
                "type": "string",
                "format": "date"
              },
              {
                "type": "string",
                "format": "date-time"
              }
            ],
            "title": "Restock Date",
            "hidden": false,
            "editable": true,
            "examples": [
              "2020-05-05"
            ],
            "description": "Date that product will be restocked"
          },
          "is_inventory_available": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Inventory Always Available",
            "hidden": false,
            "editable": true,
            "examples": [
              "Enabled"
            ],
            "enumNames": [
              "Disabled",
              "Enabled"
            ],
            "description": "Always available inventory is an alternative to quantity that allows inventory to never deplete. Enabling or disabling will toggle this feature on or off. Note that a quantity cannot be specified when provided."
          },
          "fulfillment_channel_code": {
            "enum": [
              "AMAZON_NA",
              "DEFAULT"
            ],
            "type": "string",
            "title": "Fulfillment Channel Code",
            "hidden": false,
            "editable": true,
            "examples": [
              "AMAZON_NA"
            ],
            "enumNames": [
              "AMAZON_NA",
              "DEFAULT"
            ],
            "description": "For those merchants using Amazon fulfillment services, this designates which fulfillment network will be used. Specifying a value other than DEFAULT will cancel the Merchant-fulfilled offering."
          },
          "lead_time_to_ship_max_days": {
            "type": "integer",
            "title": "Handling Time",
            "hidden": false,
            "maximum": 120,
            "minimum": 0,
            "editable": true,
            "examples": [
              "5"
            ],
            "description": "Provide the time, in days, between when you receive an order for an item and when you can ship the item"
          }
        },
        "additionalProperties": false
      },
      "title": "Fulfillment Availability",
      "minItems": 1,
      "selectors": [
        "fulfillment_channel_code"
      ],
      "description": "For those merchants using Amazon fulfillment services, please provide associated logistical information.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "item_length_width_height": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "height",
          "length",
          "width"
        ],
        "properties": {
          "width": {
            "type": "object",
            "title": "Item Width Shorter Edge",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Item Width Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches, Centimeters"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Provide the corresponding unit used to designate the item’s width."
              },
              "value": {
                "type": "number",
                "title": "Item Width Shorter Edge",
                "hidden": false,
                "maximum": 400000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "8"
                ],
                "maxLength": 5000,
                "description": "Provide the width of the item using the shorter edge."
              }
            },
            "description": "Provide the width of the item using the shorter edge.",
            "additionalProperties": false
          },
          "height": {
            "type": "object",
            "title": "Height Top to Bottom",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Item Height Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches, Centimeters"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Provide the corresponding unit used to designate the item’s height."
              },
              "value": {
                "type": "number",
                "title": "Height Top to Bottom",
                "hidden": false,
                "maximum": 400000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "8"
                ],
                "maxLength": 5000,
                "description": "Provide the height of the item from top to bottom when placed in the manner in which it is expected to be used."
              }
            },
            "description": "Provide the height of the item from top to bottom when placed in the manner in which it is expected to be used.",
            "additionalProperties": false
          },
          "length": {
            "type": "object",
            "title": "Item Length Longer Edge",
            "required": [
              "unit",
              "value"
            ],
            "properties": {
              "unit": {
                "enum": [
                  "inches"
                ],
                "type": "string",
                "title": "Item Length Unit",
                "hidden": false,
                "editable": true,
                "examples": [
                  "Inches, Centimeters"
                ],
                "enumNames": [
                  "Inches"
                ],
                "description": "Provide the corresponding unit used to designate the item’s length."
              },
              "value": {
                "type": "number",
                "title": "Item Length Longer Edge",
                "hidden": false,
                "maximum": 400000,
                "minimum": 0,
                "editable": true,
                "examples": [
                  "12"
                ],
                "maxLength": 5000,
                "description": "Provide the length of the item using the longer edge."
              }
            },
            "description": "Provide the length of the item using the longer edge.",
            "additionalProperties": false
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Item Dimensions L x W x H",
      "examples": [
        "100 Inches"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the length, width and height of the item in ready to use condition.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "main_offer_image_locator": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Main Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.offer.jpg"
            ],
            "description": "The URL where the main offer-specific image of the product is located"
          }
        },
        "additionalProperties": false
      },
      "title": "Main Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "product_site_launch_date": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "oneOf": [
              {
                "type": "string",
                "format": "date"
              },
              {
                "type": "string",
                "format": "date-time"
              }
            ],
            "title": "Product Site Launch Date",
            "hidden": false,
            "editable": true,
            "examples": [
              "2017-07-20"
            ],
            "description": "Provide the date the product launches and should first be shown on the Amazon website (YYYY-MM-DD format). PSLD does not impact buyability or pre-order logic, it is used to indicate when a product will be visible and searchable on the Amazon website"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Launch Date",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Date you wish this detail page to launch.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "california_proposition_65": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "compliance_type"
        ],
        "properties": {
          "chemical_names": {
            "type": "array",
            "items": {
              "enum": [
                "1_1_1_2_tetrachloroethane",
                "1_1_1_trichloroethane",
                "1_1_2_2_tetrachloroethane",
                "1_1_dichlor_2_2_bis_p_chlorop_ethyle_dde",
                "1_1_dichloroethane",
                "1_1_dimethylhydrazine_udmh",
                "1_2_3_trichloropropane",
                "1_2_dibromo_3_chloropropane_dbcp",
                "1_2_dichloropropane",
                "1_2_diethylhydrazine",
                "1_2_dimethylhydrazine",
                "1_3_butadiene",
                "1_3_dichloro_2_propanol_1_3_dcp",
                "1_3_dichloropropene",
                "1_3_dinitropyrene",
                "1_3_propane_sultone",
                "1_4_butanediol_dimethanesulfona_busulfan",
                "1_4_dichloro_2_butene",
                "1_4_dichloro_2_nitrobenzene",
                "1_4_dioxane",
                "1_6_dinitropyrene",
                "1_8_dinitropyrene",
                "1_2_chloroethyl_3_4_methylcyclohexyl_1_n",
                "1_2_chloroethyl_3_cyclohexyl_1_nitrosour",
                "1_5_nitrofurfurylidene_amino_2_imidazoli",
                "1_amino_2_4_dibromoanthraquinone",
                "1_amino_2_methylanthraquinone",
                "1_bromo_3_chloropropane",
                "1_bromopropane_1_bp",
                "1_butyl_glycidyl_ether",
                "1_chloro_4_nitrobenzene",
                "1_hydroxyanthraquinone",
                "1_naphthylamine",
                "1_nitropyrene",
                "2_2_bis_bromomethyl_1_3_propanediol",
                "2_3_7_8_tetrachlorodibenzo_p_dioxin_tcdd",
                "2_3_dibromo_1_propanol",
                "2_4_5_trimethy_and_its_strong_acid_salts",
                "2_4_6_trichlorophenol",
                "2_4_6_trinitrotoluene_tnt",
                "2_4_d_butyric_acid",
                "2_4_diamino_6_chloro_s_triazine_dact",
                "2_4_diaminoanisole",
                "2_4_diaminoanisole_sulfate",
                "2_4_diaminotoluene",
                "2_4_dichloro_1_nitrobenzene",
                "2_4_dinitrotoluene",
                "2_4_hexadienal_89_percent_trans_trans_is",
                "2_5_hexanedione",
                "2_6_dimethyl_n_nitrosomorpholine_dmnm",
                "2_6_dinitrotoluene",
                "2_6_xylidine_2_6_dimethylaniline",
                "2_2_formylhyd_4_5_nitro_2_furyl_thiazole",
                "2_acetylaminofluorene",
                "2_amino_4_chlorophenol",
                "2_amino_5_5_nitro_2_furyl_1_3_4_thiadiaz",
                "2_aminoanthraquinone",
                "2_aminofluorene",
                "2_bromopropane_2_bp",
                "2_chloronitrobenzene",
                "2_chloropropionic_acid",
                "2_ethylhexyl_acrylate",
                "2_methyl_1_nitroanth_of_uncertain_purity",
                "2_methylaziridine_propyleneimine",
                "2_methylimidazole",
                "2_naphthylamine",
                "2_nitrofluorene",
                "2_nitropropane",
                "2_mercaptobenzothiazole",
                "3_3_4_4_tetrachloroazobenzene",
                "3_3_dichloro_4_4_diamino_diphenyl_ether",
                "3_3_dichlorobenzidine",
                "3_3_dichlorobenzidine_dihydrochloride",
                "3_3_dimethoxybenzidine_o_dianisidine",
                "3_3_dimethoxybenzidine_dihydrochloride",
                "3_3_dimethoxybenzidine_based_dyes_metabo",
                "3_3_dimethylbenzidine_ortho_tolidine",
                "3_3_dimethylbenzidine_dihydrochloride",
                "3_3_dimethylbenzidine_based_dyes_metabol",
                "3_7_dinitrofluoranthene",
                "3_9_dinitrofluoranthene",
                "3_n_nitrosomethylamino_propionitrile",
                "3_amino_9_ethylcarbazole_hydrochloride",
                "3_chloro_2_methylpropene",
                "3_methylcholanthrene",
                "3_monochloropropane_1_2_diol_3_mcpd",
                "4_4_diaminodiphen_ether_4_4_oxydianiline",
                "4_4_methylene_bis_2_chloroaniline",
                "4_4_methylene_bis_2_methylaniline",
                "4_4_methylene_bis_n_n_dimethyl_benzenami",
                "4_4_methylenedianiline",
                "4_4_methylenedianiline_dihydrochloride",
                "4_4_thiodianiline",
                "4_n_nitrosomethyl_1_3_pyridyl_1_butanone",
                "4_amino_2_nitrophenol",
                "4_aminobiphenyl_4_aminodiphenyl",
                "4_chloro_o_phenylenediamine",
                "4_dimethylaminoazobenzene",
                "4_methylimidazole",
                "4_nitrobiphenyl",
                "4_nitropyrene",
                "4_vinyl_1_cycloh_diepoxide_vinyl_cyclohe",
                "4_vinylcyclohexene",
                "morphmethylnitrfurylidenamnooxazolidinon",
                "5_chloro_o_toluidi_its_strong_acid_salts",
                "5_methoxypsor_with_ultraviolet_a_therapy",
                "5_methylchrysene",
                "5_nitroacenaphthene",
                "6_nitrochrysene",
                "7_12_dimethylbenz_a_anthracene",
                "7_h_dibenzo_c_g_carbazole",
                "8_methoxypsor_with_ultraviolet_a_therapy",
                "a_alpha_c_2_amino_9_h_pyrido_2_3_b_indol",
                "abiraterone_acetate",
                "acetaldehyde",
                "acetamide",
                "acetazolamide",
                "acetochlor",
                "acetohydroxamic_acid",
                "acifluorfen_sodium",
                "acrylamide",
                "acrylonitrile",
                "actinomycin_d",
                "adultb",
                "af_2_2_2_furyl_3_5_nitro_2_furyl_acrylam",
                "aflatoxins",
                "alachlor",
                "alcoholic_beverages",
                "alcoholicbeverage_associatedalcoholabuse",
                "aldrin",
                "all_trans_retinoic_acid",
                "aloe_vera_non_decolor_whole_leaf_extract",
                "alprazolam",
                "altretamine",
                "amantadine_hydrochloride",
                "amikacin_sulfate",
                "aminoglutethimide",
                "aminoglycosides",
                "aminopterin",
                "amiodarone_hydrochloride",
                "amitraz",
                "amitrole",
                "amoxapine",
                "amsacrine",
                "anabolic_steroids",
                "analgesic_mixtures_containing_phenacetin",
                "androstenedione",
                "angiotensinconvertenzyme _ace_inhibitors",
                "angiote_converting_enzyme_ace_inhibitors",
                "aniline",
                "aniline_hydrochloride",
                "anisindione",
                "anthracene",
                "anthraquinone",
                "antimony_oxide_antimony_trioxide",
                "aramite",
                "areca_nut",
                "aristolochic_acids",
                "arsenic_inorganic_arsenic_compounds",
                "arsenic_inorganic_oxides",
                "asbestos",
                "aspirin",
                "atenolol",
                "atrazine",
                "auramine",
                "auranofin",
                "avermectin_b_1_abamectin",
                "azacitidine",
                "azaserine",
                "azathioprine",
                "azobenzene",
                "barbiturates",
                "beclomethasone_dipropionate",
                "benomyl",
                "benthiavalicarb_isopropyl",
                "benz_a_anthracene",
                "benzene",
                "benzidine_and_its_salts",
                "benzidine_based_dyes",
                "benzo_a_pyrene",
                "benzo_b_fluoranthene",
                "benzo_j_fluoranthene",
                "benzo_k_fluoranthene",
                "benzodiazepines",
                "benzofuran",
                "benzophenone",
                "benzotrichloride",
                "benzphetamine_hydrochloride",
                "benzyl_chloride",
                "benzyl_violet_4_b",
                "beryllium",
                "beryllium_and_beryllium_compounds",
                "beryllium_oxide",
                "beryllium_sulfate",
                "beta_butyrolactone",
                "beta_myrcene",
                "beta_propiolactone",
                "betel_quid_with_tobacco",
                "betel_quid_without_tobacco",
                "bevacizumab",
                "bis_2chloro1methylethyl_ethertechgrade",
                "bis_2_chloro_1_methyleth_ether_technical",
                "bis_2_chloroethyl_ether",
                "bis_chloromethyl_ether",
                "bischloroethyl_nitrosourea_bcnu_carmusti",
                "bisphenol_a_bpa",
                "bisphenol_s_bps",
                "bitumens_extracts_steam_refined_air_refi",
                "bracken_fern",
                "bromacil_lithium_salt",
                "bromate",
                "bromochloroacetic_acid",
                "bromodichloroacetic_acid",
                "bromodichloromethane",
                "bromoethane",
                "bromoform",
                "bromoxynil",
                "bromoxynil_octanoate",
                "butabarbital_sodium",
                "butyl_benzyl_phthalate_bbp_d",
                "butylated_hydroxyanisole",
                "c_i_acid_red_114",
                "c_i_basic_red_9_monohydrochloride",
                "c_i_direct_blue_15",
                "c_i_direct_blue_218",
                "c_i_disperse_yellow_3",
                "c_i_solvent_yellow_14",
                "cacodylic_acid",
                "cadmium",
                "cadmium_and_cadmium_compounds",
                "caffeic_acid",
                "captafol",
                "captan",
                "carbamazepine",
                "carbaryl",
                "carbazole",
                "carbon_black_airborne_unbound_particles_",
                "carbon_disulfide",
                "carbon_monoxide",
                "carbon_tetrachloride",
                "carbon_black_extracts",
                "carboplatin",
                "catechol",
                "ceramic_fiber_airbor_part_respirable_siz",
                "certain_combined_chemotherapy_for_lympho",
                "chenodiol",
                "chloral",
                "chloral_hydrate",
                "chlorambucil",
                "chloramphenicol_sodium_succinate",
                "chlorcyclizine_hydrochloride",
                "chlordane",
                "chlordecone_kepone",
                "chlordiazepoxide",
                "chlordiazepoxide_hydrochloride",
                "chlordimeform",
                "chlorendic_acid",
                "chlorinated_paraffins_average_chain_leng",
                "chloroethane_ethyl_chloride",
                "chloroform",
                "chloromethyl_methyl_ether_technical_grad",
                "chloroprene",
                "chlorothalonil",
                "chlorotrianisene",
                "chlorozotocin",
                "chlorpyrifos",
                "chromium_hexavalent_compounds",
                "chrysene",
                "ciclosporin_cyclosporin_a_cyclosporine",
                "cidofovir",
                "cinnamyl_anthranilate",
                "cisplatin",
                "citrus_red_no_2",
                "cladribine",
                "clarithromycin",
                "clobetasol_propionate",
                "clofibrate",
                "clomiphene_citrate",
                "clorazepate_dipotassium",
                "cmnp_pyrazachlor",
                "coal_tar_pitch",
                "cobalt_ii_oxide",
                "cobalt_metal_powder",
                "cobalt_sulfate",
                "cobalt_sulfate_heptahydrate",
                "coconutoilcocamidediethanolamine",
                "codeine_phosphate",
                "coke_oven_emissions",
                "colchicine",
                "conjugated_estrogens",
                "creosotes",
                "cumene",
                "cupferron",
                "cyanazine",
                "cyanidesaltsdisassociatesolution",
                "cycasin",
                "cycloate",
                "cycloheximide",
                "cyclopenta_cd_pyrene",
                "cyclophosphamide_anhydrous",
                "cyclophosphamide_hydrated",
                "cyhexatin",
                "cytarabine",
                "cytembena",
                "d_c_orange_no_17",
                "d_c_red_no_19",
                "d_c_red_no_8",
                "d_c_red_no_9",
                "dacarbazine",
                "daminozide",
                "danazol",
                "dantron_chrysazin_1_8_dihydroxyanthraqui",
                "daunomycin",
                "daunorubicin_hydrochloride",
                "ddd_dichlorodiphenyl_dichloroethane",
                "dde_dichlorodiphenyl_dichloroethylene",
                "ddt_dichlorodiphenyl_trichloroethane",
                "ddvp_dichlorvos",
                "demeclocyclin_hydrochloride_internal_use",
                "des_ethyl_atrazine_dea",
                "des_isopropyl_atrazine_dia",
                "di_2_ethylhexyl_phthalate_dehp",
                "di_isodecyl_phthalate_didp",
                "di_n_butyl_phthalate_dbp",
                "di_n_hexyl_phthalate_dn_hp",
                "di_n_propyl_isocinchom_mgk_repellent_326",
                "diazepam",
                "diazoaminobenzene",
                "diazoxide",
                "dibenz_a_c_anthracene",
                "dibenz_a_h_acridine",
                "dibenz_a_h_anthracene",
                "dibenz_a_j_acridine",
                "dibenz_a_j_anthracene",
                "dibenzanthracenes",
                "dibenzo_a_e_pyrene",
                "dibenzo_a_h_pyrene",
                "dibenzo_a_i_pyrene",
                "dibenzo_a_l_pyrene",
                "dibromoacetic_acid",
                "dibromoacetonitrile",
                "dichloroacetic_acid",
                "dichloromethane_methylene_chloride",
                "dichlorophene",
                "dichlorphenamide",
                "diclofop_methyl",
                "dicumarol",
                "dieldrin",
                "diepoxybutane",
                "diesel_engine_exhaust",
                "diethanolamine",
                "diethyl_sulfate",
                "diethylstilbestrol_des",
                "diflunisal",
                "diglycidyl_resorcinol_ether_dgre",
                "dihydroergotamine_mesylate",
                "dihydrosafrole",
                "diisononyl_phthalate_dinp",
                "diisopropyl_sulfate",
                "diltiazem_hydrochloride",
                "dimethyl_hydrogen_phosphite",
                "dimethyl_sulfate",
                "dimethylcarbamoyl_chloride",
                "dimethylvinylchloride",
                "dinitrotoluene_technical_grade",
                "dinitrotoluene_mixture_2_4_2_6",
                "dinocap",
                "dinoseb",
                "diphenylhydantoin_phenytoin",
                "diphenylhydantoin_phenytoin_sodium_salt",
                "direct_black_38_technical_grade",
                "direct_blue_6_technical_grade",
                "direct_brown_95_technical_grade",
                "disodium_cyanodithioimidocarbonate",
                "disperse_blue_1",
                "diuron",
                "doxorubicin_hydrochloride_adriamycin",
                "doxycycline_internal_use",
                "doxycycline_calcium_internal_use",
                "doxycycline_hyclate_internal_use",
                "doxycycline_monohydrate_internal_use",
                "emissions_from_combustion_of_coal",
                "emissions_from_high_temperature_unrefine",
                "endrin",
                "environmental_tobacco_smoke_ets",
                "epichlorohydrin",
                "epoxiconazole",
                "ergotamine_tartrate",
                "erionite",
                "estradiol_17_b",
                "estragole",
                "estrogen_progestogen_combined_used_as_me",
                "estrogens_steroidal",
                "estrone",
                "estropipate",
                "ethanol_in_alcoholic_beverages",
                "ethinylestradiol",
                "ethionamide",
                "ethoprop",
                "ethyl_acrylate",
                "ethyl_alcohol_in_alcoholic_beverages",
                "ethyl_dipropylthiocarbamate",
                "ethyl_methanesulfonate",
                "ethyl_4_4_dichlorobenzilate",
                "ethylbenzene",
                "ethylene_dibromide",
                "ethylene_dichloride_1_2_dichloroethane",
                "ethylene_glycol_ingested",
                "ethylene_glycol_monoethyl_ether",
                "ethylene_glycol_monoethyl_ether_acetate",
                "ethylene_glycol_monomethyl_ether",
                "ethylene_glycol_monomethyl_ether_acetate",
                "ethylene_oxide",
                "ethylene_thiourea",
                "ethyleneimine_aziridine",
                "etodolac",
                "etoposide",
                "etoposide_in_comb_with_cispla_and_bleomy",
                "etretinate",
                "fenoxaprop_ethyl",
                "fenoxycarb",
                "filgrastim",
                "fluazifop_butyl",
                "flunisolide",
                "fluoro_edenite_fibrous_amphibole",
                "fluorouracil",
                "fluoxymesterone",
                "flurazepam_hydrochloride",
                "flurbiprofen",
                "flutamide",
                "fluticasone_propionate",
                "fluvalinate",
                "folpet",
                "formaldehyde_gas",
                "fumonisin_b_1",
                "furan",
                "furazolidone",
                "furfuryl_alcohol",
                "furmecyclox",
                "fusarin_c",
                "gallium_arsenide",
                "ganciclovir",
                "ganciclovir_sodium",
                "gaso_engine_exhaust_condensates_extracts",
                "gemfibrozil",
                "gentian_violet_crystal_violet",
                "glass_wool_fibers_inhalable_and_biopersi",
                "glu_p_1_2_amino_6_meth_1_2_a_3_2_d_imida",
                "glu_p_2_2_aminodip_1_2_a_3_2_d_imidazole",
                "glycidaldehyde",
                "glycidol",
                "glycidyl_methacrylate",
                "glyphosate",
                "goldenseal_root_powder",
                "goserelin_acetate",
                "griseofulvin",
                "gyromitrin_acetaldehyde_methylformylhydr",
                "halazepam",
                "halobetasol_propionate",
                "haloperidol",
                "halothane",
                "hc_blue_1",
                "heptachlor",
                "heptachlor_epoxide",
                "herbal_remedies_containing_plant_species",
                "hexachlorobenzene",
                "hexachlorobutadiene",
                "hexachlorocyclohexane_alpha_isomer",
                "hexachlorocyclohexane_beta_isomer",
                "hexachlorocyclohexane_gamma_isomer",
                "hexachlorocyclohexane_technical_grade",
                "hexachlorodibenzodioxin",
                "hexachloroethane",
                "hexafluoroacetone",
                "hexamethylphosphoramide",
                "histrelin_acetate",
                "hydramethylnon",
                "hydrazine",
                "hydrazine_sulfate",
                "hydrazobenzene_1_2_diphenylhydrazine",
                "hydrogen_cyanide",
                "hydrogen_cyanide_hcn_and_cyanide_salts",
                "hydrogen_cyanidef",
                "hydroxyurea",
                "idarubicin_hydrochloride",
                "ifosfamide",
                "imazalil",
                "indeno_1_2_3_cd_pyrene",
                "indium_phosphide",
                "indium_tin_oxide",
                "infant_boys_ age_29_days_to_24_monthsb",
                "iodine_131",
                "iprodione",
                "iprovalicarb",
                "iq_2_amino_3_methylimida_4_5_f_quinoline",
                "iron_dextran_complex",
                "isobutyl_nitrite",
                "isoprene",
                "isopyrazam",
                "isotretinoin",
                "isoxaflutole",
                "kresoxim_methyl",
                "lactofen",
                "lasiocarpine",
                "lead",
                "lead_acetate",
                "lead_and_lead_compounds",
                "lead_phosphate",
                "lead_subacetate",
                "leather_dust",
                "leucomalachite_green",
                "leuprolide_acetate",
                "levodopa",
                "levonorgestrel_implants",
                "lindane_and_other_hexachlorocycl_isomers",
                "linuron",
                "lithium_carbonate",
                "lithium_citrate",
                "lorazepam",
                "lovastatin",
                "lynestrenol",
                "m_dinitrobenzene",
                "malathion",
                "malonaldehyde_sodium_salt",
                "mancozeb",
                "maneb",
                "me_a_alpha_c_amino_methyl_pyrido_indole",
                "mebendazole",
                "medroxyprogesterone_acetate",
                "megestrol_acetate",
                "me_iq_2_amino_3_4_dimeth_4_5_f_quinoline",
                "meiqx_amino_dimethylimidazo_quinoxaline",
                "melphalan",
                "menotropins",
                "mepanipyrim",
                "meprobamate",
                "mercaptopurine",
                "mercury_and_mercury_compounds",
                "merphalan",
                "mestranol",
                "metam_potassium",
                "methacycline_hydrochloride",
                "metham_sodium",
                "methanol",
                "methazole",
                "methimazole",
                "methotrexate",
                "methotrexate_sodium",
                "methyl_acrylate",
                "methyl_bromide_as_a_structural_fumigant",
                "methyl_carbamate",
                "methyl_chloride",
                "methyl_iodide",
                "methyl_isobutyl_ketone",
                "methyl_isobutyl_ketone_mibk",
                "methyl_isocyanate_mic",
                "methyl_mercury",
                "methyl_methanesulfonate",
                "methyl_n_butyl_ketone",
                "methylazoxymethanol",
                "methylazoxymethanol_acetate",
                "methyleugenol",
                "methylhydrazine",
                "methylhydrazine_and_its_salts",
                "methylhydrazine_sulfate",
                "methylmercury_compounds",
                "methyltestosterone",
                "methylthiouracil",
                "metiram",
                "metronidazole",
                "michlers_ketone",
                "midazolam_hydrochloride",
                "minocycline_hydrochloride_internal_use",
                "mirex",
                "misoprostol",
                "mitomycin_c",
                "mitoxantrone_hydrochloride",
                "molinate",
                "molybdenum_trioxide",
                "mon_13900_furilazole",
                "mon_4660_dichl_1_oxa_4_azaspi_4_5_decane",
                "monocrotaline",
                "mopp_vincrstprednsonnitromstrdprocarbmix",
                "mustard_gas",
                "mx_3_chloro_4_dich_5_hydr_2_5_h_furanone",
                "myclobutanil",
                "n_n_diacetylbenzidine",
                "NNBISChlorethlNapthylmnChlornapzne",
                "n_n_bis_2_chloroethyl_2_naphthyla_chlorn",
                "n_n_dimethyl_p_toluidine",
                "n_n_dimethylacetamide",
                "n_n_dimethylformamide",
                "n_4_5_nitro_2_furyl_2_thiazolyl_acetamid",
                "n_carboxymethyl_n_nitrosourea",
                "n_hexane",
                "n_methyl_n_nitro_n_nitrosoguanidine",
                "n_methylolacrylamide",
                "n_methylpyrrolidone",
                "n_nitroso_n_ethylurea",
                "n_nitroso_n_methylurea",
                "n_nitroso_n_methylurethane",
                "n_nitrosodi_n_butylamine",
                "n_nitrosodi_n_propylamine",
                "n_nitrosodiethanolamine",
                "n_nitrosodiethylamine",
                "n_nitrosodimethylamine",
                "n_nitrosodiphenylamine",
                "n_nitrosohexamethyleneimine",
                "n_nitrosomethyl_n_butylamine",
                "n_nitrosomethyl_n_decylamine",
                "n_nitrosomethyl_n_dodecylamine",
                "n_nitrosomethyl_n_heptylamine",
                "n_nitrosomethyl_n_hexylamine",
                "n_nitrosomethyl_n_nonylamine",
                "n_nitrosomethyl_n_octylamine",
                "n_nitrosomethyl_n_pentylamine",
                "n_nitrosomethyl_n_propylamine",
                "n_nitrosomethyl_n_tetradecylamine",
                "n_nitrosomethyl_n_undecylamine",
                "n_nitrosomethylethylamine",
                "n_nitrosomethylvinylamine",
                "n_nitrosomorpholine",
                "n_nitrosonornicotine",
                "n_nitrosopiperidine",
                "n_nitrosopyrrolidine",
                "n_nitrososarcosine",
                "nabam",
                "nafarelin_acetate",
                "nafenopin",
                "nalidixic_acid",
                "naphthalene",
                "neomycin_sulfate_internal_use",
                "neonatal_infant_boys_age_0_to_28_daysb",
                "netilmicin_sulfate",
                "nickel_metallic",
                "nickel_soluble_compounds",
                "nickel_acetate",
                "nickel_carbonate",
                "nickel_carbonyl",
                "nickel_compounds",
                "nickel_hydroxide",
                "nickel_oxide",
                "nickelrefinerydustpyrometallurgprocess",
                "nickel_subsulfide",
                "nickelocene",
                "nicotine",
                "nifedipine",
                "nimodipine",
                "niridazole",
                "nitrapyrin",
                "nitrilotriacetic_acid",
                "nitrilot_acid_trisodium_salt_monohydrate",
                "nitrobenzene",
                "nitrofen_technical_grade",
                "nitrofurantoin",
                "nitrofurazone",
                "nitrogen_mustard_mechlorethamine",
                "nitromustardhydrochloridemechlorethamine",
                "nitrogen_mustard_n_oxide",
                "nitrogen_mustard_n_oxide_hydrochloride",
                "nitromethane",
                "nitrous_oxide",
                "norethisterone_norethindrone",
                "norethis_norethindrone_ethinyl_estradiol",
                "norethisterone_norethindrone_mestranol",
                "norethiste_acetate_norethindrone_acetate",
                "norethynodrel",
                "norgestrel",
                "o_p_ddt",
                "o_aminoazotoluene",
                "o_anisidine",
                "o_anisidine_hydrochloride",
                "o_dinitrobenzene",
                "o_nitroanisole",
                "o_nitrotoluene",
                "o_phenylenediamine",
                "o_phenylenediamine_and_its_salts",
                "o_phenylenediamine_dihydochloride",
                "o_phenylenediamine dihydrochloride",
                "o_phenylphenate_sodium",
                "o_phenylphenol",
                "o_toluidine",
                "o_toluidine_hydrochloride",
                "ochratoxin_a",
                "oil_orange_ss",
                "oral_contraceptives_combined",
                "oral_contraceptives_sequential",
                "oryzalin",
                "oxadiazon",
                "oxazepam",
                "oxydemeton_methyl",
                "oxymetholone",
                "oxytetracycline_internal_use",
                "oxytetracycli_hydrochloride_internal_use",
                "oxythioquinox_chinomethionat",
                "p_p_ddt",
                "p_a_a_a_tetrachlorotoluene",
                "p_aminoazobenzene",
                "p_chloro_o_toluidine",
                "p_chloro_o_toluidine_hydrochloride",
                "p_chloro_o_toluidine_strong_acid_salts",
                "p_chloro_alpha_alpha_alpha_trifluorotolu",
                "p_chloroaniline",
                "p_chloroaniline_hydrochloride",
                "p_cresidine",
                "p_dichlorobenzene",
                "p_dinitrobenzene",
                "p_nitrosodiphenylamine",
                "paclitaxel",
                "palygorskite_fibers_morthn_5µm_length",
                "panfuran_s",
                "para_nitroanisole",
                "paramethadione",
                "parathion",
                "penicillamine",
                "pent_ether_mixture_de_71_technical_grade",
                "pentachlorophenol",
                "pentachlorophenolandbyproductofsynthesis",
                "pentobarbital_sodium",
                "pentosan_polysulfate_sodium",
                "pentostatin",
                "perfluorononanoicacid_pfna_salts",
                "perfluorooctane_sulfonate_pfos",
                "perfluorooctanesulfonicacid _pfos_salts",
                "perfluorooctanoic_acid_pfoa",
                "pertuzumab",
                "phenacemide",
                "phenacetin",
                "phenazopyridine",
                "phenazopyridine_hydrochloride",
                "phenesterin",
                "phenobarbital",
                "phenolphthalein",
                "phenoxybenzamine",
                "phenoxybenzamine_hydrochloride",
                "phenprocoumon",
                "phenyl_glycidyl_ether",
                "phenylhydrazine",
                "phenylhydrazine_and_its_salts",
                "phenylhydrazine_hydrochloride",
                "phenylphosphine",
                "phi_p_2_amino_1_methyl_6_phen_4_5_b_pyri",
                "pimozide",
                "pioglitazone",
                "pipobroman",
                "pirimicarb",
                "plicamycin",
                "polybrominated_biphenyls",
                "polychlorinated_biphenyls",
                "polychlorinatedbiphenyls60ormoreperent",
                "polychlorinated_dibenzo_p_dioxins",
                "polychlorinated_dibenzofurans",
                "polygeenan",
                "ponceau_3_r",
                "ponceau_mx",
                "potassium_bromate",
                "potassium_cyanide",
                "potassium_cyanidef",
                "potassium_dimethyldithiocarbamate",
                "pravastatin_sodium",
                "prednisolone_sodium_phosphate",
                "primidone",
                "procarbazine",
                "procarbazine_hydrochloride",
                "procymidone",
                "progesterone",
                "pronamide",
                "propachlor",
                "propargite",
                "propazine",
                "propoxur",
                "propylene_glycol_mono_t_butyl_ether",
                "propylene_oxide",
                "propylthiouracil",
                "pulegone",
                "pymetrozine",
                "pyridine",
                "pyrimethamine",
                "quazepam",
                "quinoline_and_its_strong_acid_salts",
                "quizalofop_ethyl",
                "radionuclides",
                "reserpine",
                "residual_heavy_fuel_oils",
                "resmethrin",
                "retinol_retinyl_esters_when_in_daily_dos",
                "ribavirin",
                "riddelliine",
                "rifampin",
                "s_s_s_tributyl_phosphorotri_tribufos_def",
                "safrole",
                "salted_fish_chinese_style",
                "secobarbital_sodium",
                "sedaxane",
                "selenium_sulfide",
                "sermorelin_acetate",
                "shale_oils",
                "silica_crystalline_airborne_particles_of",
                "silicon_carbide_whiskers",
                "simazine",
                "sodium_cyanide",
                "sodium_cyanidef",
                "sodium_dimethyldithiocarbamate",
                "sodium_fluoroacetate",
                "soots_tars_and_mineral_oils_untreated_an",
                "spirodiclofen",
                "spironolactone",
                "stanozolol",
                "sterigmatocystin",
                "streptomycin_sulfate",
                "streptozocin_streptozotocin",
                "streptozotocin_streptozocin",
                "strong_inorganic_acid_mists_containing_s",
                "styrene",
                "styrene_oxide",
                "sulfallate",
                "sulfasalazine_salicylazosulfapyridine",
                "sulfur_dioxidee",
                "sulindac",
                "talc_containing_asbestiform_fibers",
                "tamoxifen_and_its_salts",
                "tamoxifen_citrate",
                "temazepam",
                "teniposide",
                "terbacil",
                "teriparatide",
                "terrazole",
                "testosterone_and_its_esters",
                "testosterone_cypionate",
                "testosterone_enanthate",
                "tetrabromobisphenol_a",
                "tetrachloroethylene_perchloroethylene",
                "tetrachlorvinphos",
                "tetracycline_internal_use",
                "tetracycline_hydrochloride_internal_use",
                "tetracyclines_internal_use",
                "tetrafluoroethylene",
                "tetrahydrofuran",
                "tetranitromethane",
                "thalidomide",
                "thioacetamide",
                "thiodicarb",
                "thioguanine",
                "thiophanate_methyl",
                "thiouracil",
                "thiourea",
                "thorium_dioxide",
                "titanium_dioxide_airborne_unbound_partic",
                "tobacco_smoke",
                "tobacco_smoke_primary",
                "tobacco_oral_use_of_smokeless_products",
                "tobramycin_sulfate",
                "toluene",
                "toluene_diisocyanate",
                "topiramate",
                "toxaphene_polychlorinated_camphenes",
                "toxins_derived_from_fusarium_moniliforme",
                "trans_2_dimethylamino_methylimino_5_2_5_",
                "treosulfan",
                "triadimefon",
                "triamterene",
                "triazolam",
                "tributyltin_methacrylate",
                "trichlormethine_trimustine_hydrochloride",
                "trichloroacetic_acid",
                "trichloroethylene",
                "trientine_hydrochloride",
                "triforine",
                "trilostane",
                "trimethadione",
                "trimethyl_phosphate",
                "trimethylolpropane_triacrylate_technical",
                "trimetrexate_glucuronate",
                "trim_vx",
                "triphenyltin_hydroxide",
                "tris_1_3_dichloro_2_propyl_phospha_tdcpp",
                "tris_1_aziridinyl_phosp_sulfide_thiotepa",
                "tris_2_3_dibromopropyl_phosphate",
                "tris_2_chloroethyl_phosphate",
                "tris_aziridinyl_p_benzoquinone_triaziquo",
                "trp_p_1_tryptophan_p_1",
                "trp_p_2_tryptophan_p_2",
                "trypan_blue_commercial_grade",
                "unleaded_gasoline_wholly_vaporized",
                "uracil_mustard",
                "urethane_ethyl_carbamate",
                "urofollitropin",
                "valproate_valproic_acid",
                "vanadiumpentoxide_orthorhcrystallineform",
                "vinblastine_sulfate",
                "vinclozolin",
                "vincristine_sulfate",
                "vinyl_bromide",
                "vinyl_chloride",
                "vinyl_cyclohe_dioxide_4_vinyl_1_cycl_die",
                "vinyl_fluoride",
                "vinyl_trichloride_1_1_2_trichloroethane",
                "vinylidenechloride",
                "vinylidene_chloride_1_1_dichloroethylene",
                "vismodegib",
                "warfarin",
                "wood_dust",
                "zalcitabine",
                "zidovudine_azt",
                "zileuton",
                "alpha_methyl_styrene_alpha_methylstyrene"
              ],
              "type": "string",
              "enumNames": [
                "1,1,1,2-Tetrachloroethane",
                "1,1,1-trichloroethane",
                "1,1,2,2-Tetrachloroethane",
                "1,1-Dichloro-2,2-bis(p-chloropheny)ethylene (DDE)",
                "1,1-Dichloroethane",
                "1,1-Dimethylhydrazine (UDMH)",
                "1,2,3-Trichloropropane",
                "1,2-Dibromo-3-chloropropane (DBCP)",
                "1,2-Dichloropropane",
                "1,2-Diethylhydrazine",
                "1,2-Dimethylhydrazine",
                "1,3-Butadiene",
                "1,3-Dichloro-2-propanol (1,3-DCP)",
                "1,3-Dichloropropene",
                "1,3-Dinitropyrene",
                "1,3-Propane sultone",
                "1,4-Butanediol dimethanesulfonate (Busulfan)",
                "1,4-Dichloro-2-butene",
                "1,4-Dichloro-2-nitrobenzene",
                "1,4-Dioxane",
                "1,6-Dinitropyrene",
                "1,8-Dinitropyrene",
                "1-(2-Chloroethyl)-3-(4-methylcyclohexyl)-1-nitrosourea (Methyl-CCNU)",
                "1-(2-Chloroethyl)-3-cyclohexyl-1-nitrosourea (CCNU) (Lomustine)",
                "1-[(5-Nitrofurfurylidene)-amino]-2-imidazolidinone",
                "1-Amino-2,4-dibromoanthraquinone",
                "1-Amino-2-methylanthraquinone",
                "1-Bromo-3-chloropropane",
                "1-Bromopropane (1-BP)",
                "1-Butyl glycidyl ether",
                "1-Chloro-4-nitrobenzene",
                "1-Hydroxyanthraquinone",
                "1-Naphthylamine",
                "1-Nitropyrene",
                "2,2-Bis(bromomethyl)-1,3-propanediol",
                "2,3,7,8-Tetrachlorodibenzo-p-dioxin (TCDD)",
                "2,3-Dibromo-1-propanol",
                "2,4,5-Trimethylaniline and its strong acid salts",
                "2,4,6-Trichlorophenol",
                "2,4,6-Trinitrotoluene (TNT)",
                "2,4-D butyric acid",
                "2,4-Diamino-6-chloro-s-triazine (DACT)",
                "2,4-Diaminoanisole",
                "2,4-Diaminoanisole sulfate",
                "2,4-Diaminotoluene",
                "2,4-Dichloro-1-nitrobenzene",
                "2,4-Dinitrotoluene",
                "2,4-Hexadienal (89% trans, trans isomer; 11% cis, trans isomer)",
                "2,5-Hexanedione",
                "2,6-Dimethyl-N-nitrosomorpholine (DMNM)",
                "2,6-Dinitrotoluene",
                "2,6-Xylidine (2,6-Dimethylaniline)",
                "2-(2-Formylhydrazino)-4-(5-nitro-2-furyl)thiazole",
                "2-Acetylaminofluorene",
                "2-Amino-4-chlorophenol",
                "2-Amino-5-(5-nitro-2-furyl)-1,3,4-thiadiazole",
                "2-Aminoanthraquinone",
                "2-Aminofluorene",
                "2-Bromopropane (2-BP)",
                "2-Chloronitrobenzene",
                "2-Chloropropionic acid",
                "2-Ethylhexyl acrylate",
                "2-Methyl-1-nitroanthraquinone (of uncertain purity)",
                "2-Methylaziridine (Propyleneimine)",
                "2-Methylimidazole",
                "2-Naphthylamine",
                "2-Nitrofluorene",
                "2-Nitropropane",
                "2‑Mercaptobenzothiazole",
                "3,3',4,4'-Tetrachloroazobenzene",
                "3,3'-Dichloro-4,4'-diamino-diphenyl ether",
                "3,3'-Dichlorobenzidine",
                "3,3'-Dichlorobenzidine dihydrochloride",
                "3,3'-Dimethoxybenzidine (o-Dianisidine)",
                "3,3'-Dimethoxybenzidine dihydrochloride",
                "3,3'-Dimethoxybenzidine-based dyes metabolized to 3,3'-dimethoxybenzidine",
                "3,3'-Dimethylbenzidine (ortho-Tolidine)",
                "3,3'-Dimethylbenzidine dihydrochloride",
                "3,3'-Dimethylbenzidine-based dyes metabolized to 3,3'-dimethylbenzidine",
                "3,7-Dinitrofluoranthene",
                "3,9-Dinitrofluoranthene",
                "3-(N-Nitrosomethylamino) propionitrile",
                "3-Amino-9-ethylcarbazole hydrochloride",
                "3-Chloro-2-methylpropene",
                "3-Methylcholanthrene",
                "3-Monochloropropane-1,2-diol (3-MCPD)",
                "4,4'-Diaminodiphenyl ether (4,4'-Oxydianiline)",
                "4,4'-Methylene bis(2-chloroaniline)",
                "4,4'-Methylene bis(2-methylaniline)",
                "4,4'-Methylene bis(N,N-dimethyl)benzenamine",
                "4,4'-Methylenedianiline",
                "4,4'-Methylenedianiline dihydrochloride",
                "4,4'-Thiodianiline",
                "4-(N-Nitrosomethylamino)-1-(3-pyridyl)1-butanone",
                "4-Amino-2-nitrophenol",
                "4-Aminobiphenyl (4-aminodiphenyl)",
                "4-Chloro-o-phenylenediamine",
                "4-Dimethylaminoazobenzene",
                "4-Methylimidazole",
                "4-Nitrobiphenyl",
                "4-Nitropyrene",
                "4-Vinyl-1-cyclohexene diepoxide (Vinyl cyclohexenedioxide)",
                "4-Vinylcyclohexene",
                "5-(Morpholinomethyl)-3-[(5-nitrofurfuryl-idene)-amino]-2-oxazolidinone",
                "5-Chloro-o-toluidine and its strong acid salts",
                "5-Methoxypsoralen with ultraviolet A therapy",
                "5-Methylchrysene",
                "5-Nitroacenaphthene",
                "6-Nitrochrysene",
                "7,12-Dimethylbenz(a)anthracene",
                "7H-Dibenzo[c,g]carbazole",
                "8-Methoxypsoralen with ultraviolet A therapy",
                "A-alpha-C (2-Amino-9H-pyrido[2,3-b]indole)",
                "Abiraterone acetate",
                "Acetaldehyde",
                "Acetamide",
                "Acetazolamide",
                "Acetochlor",
                "Acetohydroxamic acid",
                "Acifluorfen sodium",
                "Acrylamide",
                "Acrylonitrile",
                "Actinomycin D",
                "Adultb",
                "AF-2;[2-(2-furyl)-3-(5-nitro-2-furyl)]acrylamide",
                "Aflatoxins",
                "Alachlor",
                "Alcoholic beverages",
                "Alcoholic beverages, when associated with alcohol abuse",
                "Aldrin",
                "All-trans retinoic acid",
                "Aloe Vera, non-decolorized whole leaf extract",
                "Alprazolam",
                "Altretamine",
                "Amantadine hydrochloride",
                "Amikacin sulfate",
                "Aminoglutethimide",
                "Aminoglycosides",
                "Aminopterin",
                "Amiodarone hydrochloride",
                "Amitraz",
                "Amitrole",
                "Amoxapine",
                "Amsacrine",
                "Anabolic steroids",
                "Analgesic mixtures containing Phenacetin",
                "Androstenedione",
                "Angiotensin converting enzyme  (ACE) inhibitors",
                "Angiotensin converting enzyme (ACE) inhibitors",
                "Aniline",
                "Aniline hydrochloride",
                "Anisindione",
                "Anthracene",
                "Anthraquinone",
                "Antimony oxide (Antimony trioxide)",
                "Aramite",
                "Areca nut",
                "Aristolochic acids",
                "Arsenic (inorganic arsenic compounds)",
                "Arsenic (inorganic oxides)",
                "Asbestos",
                "Aspirin",
                "Atenolol",
                "Atrazine",
                "Auramine",
                "Auranofin",
                "Avermectin B1 (Abamectin)",
                "Azacitidine",
                "Azaserine",
                "Azathioprine",
                "Azobenzene",
                "Barbiturates",
                "Beclomethasone dipropionate",
                "Benomyl",
                "Benthiavalicarb-isopropyl",
                "Benz[a]anthracene",
                "Benzene",
                "Benzidine [and its salts]",
                "Benzidine-based dyes",
                "Benzo[a]pyrene",
                "Benzo[b]fluoranthene",
                "Benzo[j]fluoranthene",
                "Benzo[k]fluoranthene",
                "Benzodiazepines",
                "Benzofuran",
                "Benzophenone",
                "Benzotrichloride",
                "Benzphetamine hydrochloride",
                "Benzyl chloride",
                "Benzyl violet 4B",
                "Beryllium",
                "Beryllium and beryllium compounds",
                "Beryllium oxide",
                "Beryllium sulfate",
                "beta-Butyrolactone",
                "beta-Myrcene",
                "beta-Propiolactone",
                "Betel quid with tobacco",
                "Betel quid without tobacco",
                "Bevacizumab",
                "Bis(2-chloro-1-methylethyl)ether,  technical grade",
                "Bis(2-chloro-1-methylethyl)ether, technical grade",
                "Bis(2-chloroethyl)ether",
                "Bis(chloromethyl)ether",
                "Bischloroethyl nitrosourea (BCNU) (Carmustine)",
                "Bisphenol A (BPA)",
                "Bisphenol S (BPS)",
                "Bitumens, extracts of steam-refined and air refined",
                "Bracken fern",
                "Bromacil lithium salt",
                "Bromate",
                "Bromochloroacetic acid",
                "Bromodichloroacetic acid",
                "Bromodichloromethane",
                "Bromoethane",
                "Bromoform",
                "Bromoxynil",
                "Bromoxynil octanoate",
                "Butabarbital sodium",
                "Butyl benzyl phthalate (BBP)d",
                "Butylated hydroxyanisole",
                "C.I. Acid Red 114",
                "C.I. Basic Red 9 monohydrochloride",
                "C.I. Direct Blue 15",
                "C.I. Direct Blue 218",
                "C.I. Disperse Yellow 3",
                "C.I. Solvent Yellow 14",
                "Cacodylic acid",
                "Cadmium",
                "Cadmium and cadmium compounds",
                "Caffeic acid",
                "Captafol",
                "Captan",
                "Carbamazepine",
                "Carbaryl",
                "Carbazole",
                "Carbon black (airborne, unbound particles of respirable size)",
                "Carbon disulfide",
                "Carbon monoxide",
                "Carbon tetrachloride",
                "Carbon-black extracts",
                "Carboplatin",
                "Catechol",
                "Ceramic fibers (airborne particles of respirable size)",
                "Certain combined chemotherapy for lymphomas",
                "Chenodiol",
                "Chloral",
                "Chloral hydrate",
                "Chlorambucil",
                "Chloramphenicol sodium succinate",
                "Chlorcyclizine hydrochloride",
                "Chlordane",
                "Chlordecone (Kepone)",
                "Chlordiazepoxide",
                "Chlordiazepoxide hydrochloride",
                "Chlordimeform",
                "Chlorendic acid",
                "Chlorinated paraffins (Average chain length, C12;approximately 60 percent chlorine by weight)",
                "Chloroethane (Ethyl chloride)",
                "Chloroform",
                "Chloromethyl methyl ether (technical grade)",
                "Chloroprene",
                "Chlorothalonil",
                "Chlorotrianisene",
                "Chlorozotocin",
                "Chlorpyrifos",
                "Chromium (hexavalent compounds)",
                "Chrysene",
                "Ciclosporin (Cyclosporin A; Cyclosporine)",
                "Cidofovir",
                "Cinnamyl anthranilate",
                "Cisplatin",
                "Citrus Red No. 2",
                "Cladribine",
                "Clarithromycin",
                "Clobetasol propionate",
                "Clofibrate",
                "Clomiphene citrate",
                "Clorazepate dipotassium",
                "CMNP (pyrazachlor)",
                "Coal-tar pitch",
                "Cobalt [II] oxide",
                "Cobalt metal powder",
                "Cobalt sulfate",
                "Cobalt sulfate heptahydrate",
                "Coconut oil diethanolamine condensate (cocamide diethanolamine)",
                "Codeine phosphate",
                "Coke oven emissions",
                "Colchicine",
                "Conjugated estrogens",
                "Creosotes",
                "Cumene",
                "Cupferron",
                "Cyanazine",
                "Cyanide salts that readily dissociate in solution (expressed as cyanide)f",
                "Cycasin",
                "Cycloate",
                "Cycloheximide",
                "Cyclopenta[cd]pyrene",
                "Cyclophosphamide (anhydrous)",
                "Cyclophosphamide (hydrated)",
                "Cyhexatin",
                "Cytarabine",
                "Cytembena",
                "D&C Orange No. 17",
                "D&C Red No. 19",
                "D&C Red No. 8",
                "D&C Red No. 9",
                "Dacarbazine",
                "Daminozide",
                "Danazol",
                "Dantron (Chrysazin; 1,8-Dihydroxyanthraquinone)",
                "Daunomycin",
                "Daunorubicin hydrochloride",
                "DDD (Dichlorodiphenyl-dichloroethane)",
                "DDE (Dichlorodiphenyl-dichloroethylene)",
                "DDT (Dichlorodiphenyl-trichloroethane)",
                "DDVP (Dichlorvos)",
                "Demeclocycline hydrochloride (internal use)",
                "Des-ethyl atrazine (DEA)",
                "Des-isopropyl atrazine (DIA)",
                "Di(2-ethylhexyl)phthalate (DEHP)",
                "Di-isodecyl phthalate (DIDP)",
                "Di-n-butyl phthalate (DBP)",
                "Di-n-hexyl phthalate (DnHP)",
                "Di-n-propyl isocinchomeronate (MGK Repellent 326)",
                "Diazepam",
                "Diazoaminobenzene",
                "Diazoxide",
                "Dibenz[a,c]anthracene",
                "Dibenz[a,h]acridine",
                "Dibenz[a,h]anthracene",
                "Dibenz[a,j]acridine",
                "Dibenz[a,j]anthracene",
                "Dibenzanthracenes",
                "Dibenzo[a,e]pyrene",
                "Dibenzo[a,h]pyrene",
                "Dibenzo[a,i]pyrene",
                "Dibenzo[a,l]pyrene",
                "Dibromoacetic acid",
                "Dibromoacetonitrile",
                "Dichloroacetic acid",
                "Dichloromethane (Methylene chloride)",
                "Dichlorophene",
                "Dichlorphenamide",
                "Diclofop-methyl",
                "Dicumarol",
                "Dieldrin",
                "Diepoxybutane",
                "Diesel engine exhaust",
                "Diethanolamine",
                "Diethyl sulfate",
                "Diethylstilbestrol (DES)",
                "Diflunisal",
                "Diglycidyl resorcinol ether (DGRE)",
                "Dihydroergotamine mesylate",
                "Dihydrosafrole",
                "Diisononyl phthalate (DINP)",
                "Diisopropyl sulfate",
                "Diltiazem hydrochloride",
                "Dimethyl hydrogen phosphite",
                "Dimethyl sulfate",
                "Dimethylcarbamoyl chloride",
                "Dimethylvinylchloride",
                "Dinitrotoluene (technical grade)",
                "Dinitrotoluene mixture, 2,4-/2,6-",
                "Dinocap",
                "Dinoseb",
                "Diphenylhydantoin (Phenytoin)",
                "Diphenylhydantoin (Phenytoin), sodium salt",
                "Direct Black 38 (technical grade)",
                "Direct Blue 6 (technical grade)",
                "Direct Brown 95 (technical grade)",
                "Disodium cyanodithioimidocarbonate",
                "Disperse Blue 1",
                "Diuron",
                "Doxorubicin hydrochloride (Adriamycin)",
                "Doxycycline (internal use)",
                "Doxycycline calcium (internal use)",
                "Doxycycline hyclate (internal use)",
                "Doxycycline monohydrate (internal use)",
                "Emissions from combustion of coal",
                "Emissions from high-temperature unrefined rapeseed oil",
                "Endrin",
                "Environmental tobacco smoke (ETS)",
                "Epichlorohydrin",
                "Epoxiconazole",
                "Ergotamine tartrate",
                "Erionite",
                "Estradiol 17B",
                "Estragole",
                "Estrogen-progestogen (combined) used as menopausal therapy",
                "Estrogens, steroidal",
                "Estrone",
                "Estropipate",
                "Ethanol in alcoholic beverages",
                "Ethinylestradiol",
                "Ethionamide",
                "Ethoprop",
                "Ethyl acrylate",
                "Ethyl alcohol in alcoholic beverages",
                "Ethyl dipropylthiocarbamate",
                "Ethyl methanesulfonate",
                "Ethyl-4,4'-dichlorobenzilate",
                "Ethylbenzene",
                "Ethylene dibromide",
                "Ethylene dichloride (1,2-Dichloroethane)",
                "Ethylene glycol (ingested)",
                "Ethylene glycol monoethyl ether",
                "Ethylene glycol monoethyl ether acetate",
                "Ethylene glycol monomethyl ether",
                "Ethylene glycol monomethyl ether acetate",
                "Ethylene oxide",
                "Ethylene thiourea",
                "Ethyleneimine (Aziridine)",
                "Etodolac",
                "Etoposide",
                "Etoposide in combination with cisplatin and bleomycin",
                "Etretinate",
                "Fenoxaprop ethyl",
                "Fenoxycarb",
                "Filgrastim",
                "Fluazifop butyl",
                "Flunisolide",
                "Fluoro-edenite fibrous amphibole",
                "Fluorouracil",
                "Fluoxymesterone",
                "Flurazepam hydrochloride",
                "Flurbiprofen",
                "Flutamide",
                "Fluticasone propionate",
                "Fluvalinate",
                "Folpet",
                "Formaldehyde (gas)",
                "Fumonisin B1",
                "Furan",
                "Furazolidone",
                "Furfuryl alcohol",
                "Furmecyclox",
                "Fusarin C",
                "Gallium arsenide",
                "Ganciclovir",
                "Ganciclovir sodium",
                "Gasoline engine exhaust (condensates/extracts)",
                "Gemfibrozil",
                "Gentian violet (Crystal violet)",
                "Glass wool fibers (inhalable and biopersistent)",
                "Glu-P-1 (2-Amino-6-methyldipyrido[1,2- a:3',2'-d]imidazole)",
                "Glu-P-2 (2-Aminodipyrido[1,2-a:3',2'-d]imidazole)",
                "Glycidaldehyde",
                "Glycidol",
                "Glycidyl methacrylate",
                "Glyphosate",
                "Goldenseal root powder",
                "Goserelin acetate",
                "Griseofulvin",
                "Gyromitrin (Acetaldehyde methylformylhydrazone)",
                "Halazepam",
                "Halobetasol propionate",
                "Haloperidol",
                "Halothane",
                "HC Blue 1",
                "Heptachlor",
                "Heptachlor epoxide",
                "Herbal remedies containing plant species of the genus Aristolochia",
                "Hexachlorobenzene",
                "Hexachlorobutadiene",
                "Hexachlorocyclohexane (alpha isomer)",
                "Hexachlorocyclohexane (beta isomer)",
                "Hexachlorocyclohexane (gamma isomer)",
                "Hexachlorocyclohexane (technical grade)",
                "Hexachlorodibenzodioxin",
                "Hexachloroethane",
                "Hexafluoroacetone",
                "Hexamethylphosphoramide",
                "Histrelin acetate",
                "Hydramethylnon",
                "Hydrazine",
                "Hydrazine sulfate",
                "Hydrazobenzene (1,2-Diphenylhydrazine)",
                "Hydrogen cyanide",
                "Hydrogen cyanide (HCN) and cyanide salts (CN salts)",
                "Hydrogen cyanidef",
                "Hydroxyurea",
                "Idarubicin hydrochloride",
                "Ifosfamide",
                "Imazalil",
                "Indeno[1,2,3-cd]pyrene",
                "Indium phosphide",
                "Indium tin oxide",
                "Infant boys, age 29 days to 24 monthsb",
                "Iodine-131",
                "Iprodione",
                "Iprovalicarb",
                "IQ (2-Amino-3-methylimidazo[4,5-f] quinoline)",
                "Iron dextran complex",
                "Isobutyl nitrite",
                "Isoprene",
                "Isopyrazam",
                "Isotretinoin",
                "Isoxaflutole",
                "Kresoxim-methyl",
                "Lactofen",
                "Lasiocarpine",
                "Lead",
                "Lead acetate",
                "Lead and lead compounds",
                "Lead phosphate",
                "Lead subacetate",
                "Leather dust",
                "leucomalachite green",
                "Leuprolide acetate",
                "Levodopa",
                "Levonorgestrel implants",
                "Lindane and other hexachlorocyclohexane isomers",
                "Linuron",
                "Lithium carbonate",
                "Lithium citrate",
                "Lorazepam",
                "Lovastatin",
                "Lynestrenol",
                "m-Dinitrobenzene",
                "Malathion",
                "Malonaldehyde, sodium salt",
                "Mancozeb",
                "Maneb",
                "Me-A-alpha-C (2-Amino-3-methyl-9H-pyrido[2,3-b]indole)",
                "Mebendazole",
                "Medroxyprogesterone acetate",
                "Megestrol acetate",
                "MeIQ (2-Amino-3,4-dimethylimidazo[4,5-f]quinoline)",
                "MeIQx (2-Amino-3,8-dimethylimidazo[4,5-f]quinoxaline)",
                "Melphalan",
                "Menotropins",
                "Mepanipyrim",
                "Meprobamate",
                "Mercaptopurine",
                "Mercury and mercury compounds",
                "Merphalan",
                "Mestranol",
                "Metam potassium",
                "Methacycline hydrochloride",
                "Metham sodium",
                "Methanol",
                "Methazole",
                "Methimazole",
                "Methotrexate",
                "Methotrexate sodium",
                "Methyl acrylate",
                "Methyl bromide, as a structural fumigant",
                "Methyl carbamate",
                "Methyl chloride",
                "Methyl iodide",
                "Methyl isobutyl ketone",
                "Methyl isobutyl ketone (MIBK)",
                "Methyl isocyanate (MIC)",
                "Methyl mercury",
                "Methyl methanesulfonate",
                "Methyl-n-butyl ketone",
                "Methylazoxymethanol",
                "Methylazoxymethanol acetate",
                "Methyleugenol",
                "Methylhydrazine",
                "Methylhydrazine and its salts",
                "Methylhydrazine sulfate",
                "Methylmercury compounds",
                "Methyltestosterone",
                "Methylthiouracil",
                "Metiram",
                "Metronidazole",
                "Michler's ketone",
                "Midazolam hydrochloride",
                "Minocycline hydrochloride (internal use)",
                "Mirex",
                "Misoprostol",
                "Mitomycin C",
                "Mitoxantrone hydrochloride",
                "Molinate",
                "Molybdenum trioxide",
                "MON 13900 (furilazole)",
                "MON 4660 (dichloroacetyl-1-oxa-4-azaspiro(4,5)-decane",
                "Monocrotaline",
                "MOPP (vincristine-prednisone-nitrogen mustard-procarbazine mixture)",
                "Mustard Gas",
                "MX (3-chloro-4-dichloromethyl-5-hydroxy-2(5H)-furanone)",
                "Myclobutanil",
                "N,N'-Diacetylbenzidine",
                "N,N-Bis(2-chloroethyl)-2-naphthylamine  (Chlornapazine)",
                "N,N-Bis(2-chloroethyl)-2-naphthylamine (Chlornapazine)",
                "N,N-Dimethyl-p-toluidine",
                "N,N-Dimethylacetamide",
                "N,N-Dimethylformamide",
                "N-[4-(5-Nitro-2-furyl)-2-thiazolyl]acetamide",
                "N-Carboxymethyl-N-nitrosourea",
                "n-Hexane",
                "N-Methyl-N'-nitro-N-nitrosoguanidine",
                "N-Methylolacrylamide",
                "N-Methylpyrrolidone",
                "N-Nitroso-N-ethylurea",
                "N-Nitroso-N-methylurea",
                "N-Nitroso-N-methylurethane",
                "N-Nitrosodi-n-butylamine",
                "N-Nitrosodi-n-propylamine",
                "N-Nitrosodiethanolamine",
                "N-Nitrosodiethylamine",
                "N-Nitrosodimethylamine",
                "N-Nitrosodiphenylamine",
                "N-Nitrosohexamethyleneimine",
                "N-Nitrosomethyl-n-butylamine",
                "N-Nitrosomethyl-n-decylamine",
                "N-Nitrosomethyl-n-dodecylamine",
                "N-Nitrosomethyl-n-heptylamine",
                "N-Nitrosomethyl-n-hexylamine",
                "N-Nitrosomethyl-n-nonylamine",
                "N-Nitrosomethyl-n-octylamine",
                "N-Nitrosomethyl-n-pentylamine",
                "N-Nitrosomethyl-n-propylamine",
                "N-Nitrosomethyl-n-tetradecylamine",
                "N-Nitrosomethyl-n-undecylamine",
                "N-Nitrosomethylethylamine",
                "N-Nitrosomethylvinylamine",
                "N-Nitrosomorpholine",
                "N-Nitrosonornicotine",
                "N-Nitrosopiperidine",
                "N-Nitrosopyrrolidine",
                "N-Nitrososarcosine",
                "Nabam",
                "Nafarelin acetate",
                "Nafenopin",
                "Nalidixic acid",
                "Naphthalene",
                "Neomycin sulfate (internal use)",
                "Neonatal infant boys, age 0 to 28 daysb",
                "Netilmicin sulfate",
                "Nickel (Metallic)",
                "Nickel (soluble compounds)",
                "Nickel acetate",
                "Nickel carbonate",
                "Nickel carbonyl",
                "Nickel compounds",
                "Nickel hydroxide",
                "Nickel oxide",
                "Nickel refinery dust from the pyrometallurgical process",
                "Nickel subsulfide",
                "Nickelocene",
                "Nicotine",
                "Nifedipine",
                "Nimodipine",
                "Niridazole",
                "Nitrapyrin",
                "Nitrilotriacetic acid",
                "Nitrilotriacetic acid, trisodium salt monohydrate",
                "Nitrobenzene",
                "Nitrofen (technical grade)",
                "Nitrofurantoin",
                "Nitrofurazone",
                "Nitrogen mustard (Mechlorethamine)",
                "Nitrogen mustard hydrochloride (Mechlorethamine hydrochloride)",
                "Nitrogen mustard N-oxide",
                "Nitrogen mustard N-oxide hydrochloride",
                "Nitromethane",
                "Nitrous oxide",
                "Norethisterone (Norethindrone)",
                "Norethisterone (Norethindrone) /Ethinyl estradiol",
                "Norethisterone (Norethindrone) /Mestranol",
                "Norethisterone acetate (Norethindrone acetate)",
                "Norethynodrel",
                "Norgestrel",
                "o,p'-DDT",
                "o-Aminoazotoluene",
                "o-Anisidine",
                "o-Anisidine hydrochloride",
                "o-Dinitrobenzene",
                "o-Nitroanisole",
                "o-Nitrotoluene",
                "o-Phenylenediamine",
                "o-Phenylenediamine and its salts",
                "o-Phenylenediamine dihydochloride",
                "o-Phenylenediamine dihydrochloride",
                "o-Phenylphenate, sodium",
                "o-Phenylphenol",
                "o-Toluidine",
                "o-Toluidine hydrochloride",
                "Ochratoxin A",
                "Oil Orange SS",
                "Oral contraceptives, combined",
                "Oral contraceptives, sequential",
                "Oryzalin",
                "Oxadiazon",
                "Oxazepam",
                "Oxydemeton methyl",
                "Oxymetholone",
                "Oxytetracycline (internal use)",
                "Oxytetracycline hydrochloride (internal use)",
                "Oxythioquinox (Chinomethionat)",
                "p,p'-DDT",
                "p-a,a,a-Tetrachlorotoluene",
                "p-Aminoazobenzene",
                "p-Chloro-o-toluidine",
                "p-Chloro-o-toluidine, hydrochloride",
                "p-Chloro-o-toluidine, strong acid salts of",
                "p-chloro-α,α,α-trifluorotoluene (para-Chlorobenzotrifluoride, PCBTF)",
                "p-Chloroaniline",
                "p-Chloroaniline hydrochloride",
                "p-Cresidine",
                "p-Dichlorobenzene",
                "p-Dinitrobenzene",
                "p-Nitrosodiphenylamine",
                "Paclitaxel",
                "Palygorskite fibers (> 5µm in length)",
                "Panfuran S",
                "para-Nitroanisole",
                "Paramethadione",
                "Parathion",
                "Penicillamine",
                "pentabromodiphenyl ether mixture [DE-71 (technical grade)]",
                "Pentachlorophenol",
                "Pentachlorophenol and by-products of its synthesis (complex mixture)",
                "Pentobarbital sodium",
                "Pentosan polysulfate sodium",
                "Pentostatin",
                "Perfluorononanoic acid (PFNA) and its salts",
                "Perfluorooctane sulfonate (PFOS)",
                "Perfluorooctane sulfonic acid (PFOS) and its salts and transformation and degradation precursors",
                "Perfluorooctanoic acid (PFOA)",
                "Pertuzumab",
                "Phenacemide",
                "Phenacetin",
                "Phenazopyridine",
                "Phenazopyridine hydrochloride",
                "Phenesterin",
                "Phenobarbital",
                "Phenolphthalein",
                "Phenoxybenzamine",
                "Phenoxybenzamine hydrochloride",
                "Phenprocoumon",
                "Phenyl glycidyl ether",
                "Phenylhydrazine",
                "Phenylhydrazine and its salts",
                "Phenylhydrazine hydrochloride",
                "Phenylphosphine",
                "PhiP(2-Amino-1-methyl-6-phenylimidazol[4,5-b]pyridine)",
                "Pimozide",
                "Pioglitazone",
                "Pipobroman",
                "Pirimicarb",
                "Plicamycin",
                "Polybrominated biphenyls",
                "Polychlorinated biphenyls",
                "Polychlorinated biphenyls (containing 60 or more percent chlorine by molecular weight)",
                "Polychlorinated dibenzo-p-dioxins",
                "Polychlorinated dibenzofurans",
                "Polygeenan",
                "Ponceau 3R",
                "Ponceau MX",
                "Potassium bromate",
                "Potassium cyanide",
                "Potassium cyanidef",
                "Potassium dimethyldithiocarbamate",
                "Pravastatin sodium",
                "Prednisolone sodium phosphate",
                "Primidone",
                "Procarbazine",
                "Procarbazine hydrochloride",
                "Procymidone",
                "Progesterone",
                "Pronamide",
                "Propachlor",
                "Propargite",
                "Propazine",
                "Propoxur",
                "Propylene glycol mono-t-butyl ether",
                "Propylene oxide",
                "Propylthiouracil",
                "Pulegone",
                "Pymetrozine",
                "Pyridine",
                "Pyrimethamine",
                "Quazepam",
                "Quinoline and its strong acid salts",
                "Quizalofop-ethyl",
                "Radionuclides",
                "Reserpine",
                "Residual (heavy) fuel oils",
                "Resmethrin",
                "Retinol/retinyl esters, when in daily dosages in excess of 10,000 IU, or 3,000 retinol equivalents.",
                "Ribavirin",
                "Riddelliine",
                "Rifampin",
                "S,S,S-Tributyl phosphorotrithioate (Tribufos, DEF)",
                "Safrole",
                "Salted fish, Chinese-style",
                "Secobarbital sodium",
                "Sedaxane",
                "Selenium sulfide",
                "Sermorelin acetate",
                "Shale-oils",
                "Silica, crystalline (airborne particles of respirable size)",
                "Silicon carbide whiskers",
                "Simazine",
                "Sodium cyanide",
                "Sodium cyanidef",
                "Sodium dimethyldithiocarbamate",
                "Sodium fluoroacetate",
                "Soots, tars, and mineral oils (untreated and mildly treated oils and used engine oils)",
                "Spirodiclofen",
                "Spironolactone",
                "Stanozolol",
                "Sterigmatocystin",
                "Streptomycin sulfate",
                "Streptozocin (streptozotocin)",
                "Streptozotocin (streptozocin)",
                "Strong inorganic acid mists containing sulfuric acid",
                "Styrene",
                "Styrene oxide",
                "Sulfallate",
                "Sulfasalazine (Salicylazosulfapyridine)",
                "Sulfur dioxidee",
                "Sulindac",
                "Talc containing asbestiform fibers",
                "Tamoxifen and its salts",
                "Tamoxifen citrate",
                "Temazepam",
                "Teniposide",
                "Terbacil",
                "Teriparatide",
                "Terrazole",
                "Testosterone and its esters",
                "Testosterone cypionate",
                "Testosterone enanthate",
                "Tetrabromobisphenol A",
                "Tetrachloroethylene (Perchloroethylene)",
                "Tetrachlorvinphos",
                "Tetracycline (internal use)",
                "Tetracycline hydrochloride (internal use)",
                "Tetracyclines (internal use)",
                "Tetrafluoroethylene",
                "Tetrahydrofuran",
                "Tetranitromethane",
                "Thalidomide",
                "Thioacetamide",
                "Thiodicarb",
                "Thioguanine",
                "Thiophanate methyl",
                "Thiouracil",
                "Thiourea",
                "Thorium dioxide",
                "Titanium dioxide (airborne, unbound particles of respirable size)",
                "Tobacco smoke",
                "Tobacco smoke (primary)",
                "Tobacco, oral use of smokeless products",
                "Tobramycin sulfate",
                "Toluene",
                "Toluene diisocyanate",
                "Topiramate",
                "Toxaphene (Polychlorinated camphenes)",
                "Toxins derived from Fusarium moniliforme (Fusarium verticillioides)",
                "trans-2-[(Dimethylamino)methylimino]-5-[2-(5-nitro-2-furyl)vinyl]-1,3,4-oxadiazole",
                "Treosulfan",
                "Triadimefon",
                "Triamterene",
                "Triazolam",
                "Tributyltin methacrylate",
                "Trichlormethine (Trimustine hydrochloride)",
                "Trichloroacetic acid",
                "Trichloroethylene",
                "Trientine hydrochloride",
                "Triforine",
                "Trilostane",
                "Trimethadione",
                "Trimethyl phosphate",
                "Trimethylolpropane triacrylate, technical grade",
                "Trimetrexate glucuronate",
                "TRIM® VX",
                "Triphenyltin hydroxide",
                "Tris(1,3-dichloro-2-propyl) phosphate (TDCPP)",
                "Tris(1-aziridinyl)phosphine sulfide (Thiotepa)",
                "Tris(2,3-dibromopropyl)phosphate",
                "Tris(2-chloroethyl) phosphate",
                "Tris(aziridinyl)-p-benzoquinone (Triaziquone)",
                "Trp-P-1 (Tryptophan-P-1)",
                "Trp-P-2 (Tryptophan-P-2)",
                "Trypan blue (commercial grade)",
                "Unleaded gasoline (wholly vaporized)",
                "Uracil mustard",
                "Urethane (Ethyl carbamate)",
                "Urofollitropin",
                "Valproate (Valproic acid)",
                "Vanadium pentoxide (orthorhombic crystalline form)",
                "Vinblastine sulfate",
                "Vinclozolin",
                "Vincristine sulfate",
                "Vinyl bromide",
                "Vinyl chloride",
                "Vinyl cyclohexene dioxide (4-Vinyl-1-cyclohexene diepoxide)",
                "Vinyl fluoride",
                "Vinyl trichloride (1,1,2-Trichloroethane)",
                "Vinylidene chloride \r\r\n(1,1-Dichloroethylene)",
                "Vinylidene chloride (1,1-Dichloroethylene)",
                "Vismodegib",
                "Warfarin",
                "Wood dust",
                "Zalcitabine",
                "Zidovudine (AZT)",
                "Zileuton",
                "α-Methyl styrene (alpha-Methylstyrene)"
              ]
            },
            "title": "California Proposition 65 Chemical Name(s)",
            "hidden": false,
            "editable": true,
            "examples": [
              "Lead"
            ],
            "maxItems": 5,
            "minItems": 1,
            "description": "If you selected the Food, Furniture, or Chemical warning you must indicate a chemical(s). You certify that the chemical(s) satisfies legal requirements and that you’ll remove a chemical previously provided only if it is no longer legally required."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "compliance_type": {
            "enum": [
              "alcoholic_beverage",
              "chemical",
              "diesel_engines",
              "food",
              "furniture",
              "on_product_cancer",
              "on_product_combined_cancer_reproductive",
              "on_product_reproductive",
              "passenger_or_off_road_vehicle",
              "raw_wood",
              "recreational_vessel"
            ],
            "type": "string",
            "title": "California Proposition 65 Warning Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "Furniture"
            ],
            "enumNames": [
              "Alcoholic Beverage",
              "Chemical",
              "Diesel Engines",
              "Food",
              "Furniture",
              "On Product Cancer",
              "On Product Combined Cancer Reproductive",
              "On Product Reproductive",
              "Passenger or Off Road Vehicle",
              "Raw Wood",
              "Recreational Vessel"
            ],
            "description": "Select the warning type applicable to your product, if any. You certify that the warning provided satisfies legal requirements and that you’ll remove a warning previously provided only if it is no longer legally required."
          }
        },
        "additionalProperties": false
      },
      "title": "California Proposition 65",
      "examples": [
        "Furniture; Lead"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the Proposition 65 warning information applicable to your product, if any. By removing or changing the information you certify that the previously provided warning information is no longer legally required",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "specific_uses_for_product": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Chopping",
                  "Grinding",
                  "Milling"
                ],
                "type": "string",
                "enumNames": [
                  "Chopping",
                  "Grinding",
                  "Milling"
                ]
              }
            ],
            "title": "Specific Uses for Product",
            "hidden": false,
            "editable": true,
            "examples": [
              "Dry Sanding"
            ],
            "maxLength": 3957,
            "description": "Select from the list of suggested values the conditions, or usages for which the product is specifically intended."
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Specific Uses For Product",
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Select from the list of suggested values the conditions, or usages for which the product is specifically intended.",
      "maxUniqueItems": 37,
      "minUniqueItems": 1
    },
    "main_product_image_locator": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Main Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.main.jpg"
            ],
            "description": "The URL where the main offer-specific image of the product is located."
          }
        },
        "additionalProperties": false
      },
      "title": "Main Product Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Main Product Image Locator of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "gpsr_manufacturer_reference": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "gpsr_manufacturer_email_address": {
            "type": "string",
            "title": "Manufacturer’s Email or Electronic Address",
            "hidden": false,
            "editable": true,
            "examples": [
              "abc@example.com"
            ],
            "maxLength": 100,
            "description": "Provide the email address or URL of the manufacturer to comply with the EU General Product Safety Regulation (GPSR). If you’ve already submitted this manufacturer’s information in the past, make sure you use the same email or URL."
          }
        },
        "additionalProperties": false
      },
      "title": "GPSR Manufacturer Reference",
      "examples": [
        "abc@example.com"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the email address or URL of the manufacturer to comply with the EU General Product Safety Regulation (GPSR). If you’ve already submitted this manufacturer’s information in the past, make sure you use the same email or URL.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "number_of_lithium_ion_cells": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Number of Lithium-ion Cells",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "7"
            ],
            "description": "Specify the total number of Lithium-ion cells in the product where the cell isn't contained in an encased battery. For example, an AA battery is considered a cell"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Number of Lithium-ion Cells",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Total number of Lithium cells (of type \"Ion\") in the product, where the cell isn't contained in an encased battery.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_offer_image_locator_1": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_offer_image_locator_2": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_offer_image_locator_3": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_offer_image_locator_4": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_offer_image_locator_5": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image Location",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Offer Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the location and source of the image",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "recommended_uses_for_product": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "language_tag",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "anyOf": [
              {
                "type": "string"
              },
              {
                "enum": [
                  "Chopping",
                  "Grinding",
                  "Mincing",
                  "Mixing",
                  "Seed Removal",
                  "Skin Removal",
                  "Slicing"
                ],
                "type": "string",
                "enumNames": [
                  "Chopping",
                  "Grinding",
                  "Mincing",
                  "Mixing",
                  "Seed Removal",
                  "Skin Removal",
                  "Slicing"
                ]
              }
            ],
            "title": "Recommended Uses For Product",
            "hidden": false,
            "editable": true,
            "examples": [
              "Cycling"
            ],
            "maxLength": 2329,
            "description": "Specify the recommended uses for the product"
          },
          "language_tag": {
            "$ref": "#/$defs/language_tag"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Recommended Uses For Product",
      "examples": [
        "Cycling"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "language_tag"
      ],
      "description": "Specify the recommended uses for the product",
      "maxUniqueItems": 11,
      "minUniqueItems": 1
    },
    "swatch_product_image_locator": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Swatch Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.swatch.jpg"
            ],
            "description": "The URL where an image of a color swatch from the product is located"
          }
        },
        "additionalProperties": false
      },
      "title": "Swatch Product Image Locator",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Swatch Product Image Locator of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "child_parent_sku_relationship": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "child_relationship_type"
        ],
        "properties": {
          "parent_sku": {
            "type": "string",
            "title": "Parent SKU",
            "hidden": false,
            "editable": true,
            "examples": [
              "ABC123"
            ],
            "maxLength": 40,
            "minLength": 1,
            "description": "The SKU of the parent item",
            "maxUtf8ByteLength": 40,
            "minUtf8ByteLength": 1
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "child_relationship_type": {
            "enum": [
              "variation"
            ],
            "type": "string",
            "title": "Child Relationship Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "accessory"
            ],
            "enumNames": [
              "Variation"
            ],
            "description": "The relationship that the child has to the parent"
          }
        },
        "additionalProperties": false
      },
      "title": "Child Parent Sku Relationship",
      "examples": [
        "Accessory"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Child Parent Sku Relationship of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "dsa_responsible_party_address": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Responsible Person's Email or Electronic Address",
            "hidden": false,
            "editable": true,
            "examples": [
              "rsp-email@example.com"
            ],
            "maxLength": 1000,
            "description": "Provide the email address or URL for the EU Responsible Person, representing the product in compliance with EU regulations."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Responsible Person's Email or Electronic Address",
      "examples": [
        "rsp-email@example.com"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the email address or URL for the EU Responsible Person, representing the product in compliance with EU regulations.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "number_of_lithium_metal_cells": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "type": "integer",
            "title": "Number of Lithium Metal Cells",
            "hidden": false,
            "minimum": 0,
            "editable": true,
            "examples": [
              "7"
            ],
            "description": "Specify the total number of Lithium Metal cells in the product where the cell isn't contained in an encased battery (e.g. coin cells)"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Number of Lithium Metal Cells",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Total number of Lithium cells (of type \"Metal\") in the product, where the cell isn't contained in an encased battery.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_1": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 1",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 1 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_2": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 2",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 2 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_3": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 3",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 3 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_4": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 4",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 4 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_5": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 5",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 5 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_6": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 6",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 6 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_7": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 7",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 7 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "other_product_image_locator_8": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "media_location"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "media_location": {
            "type": "string",
            "title": "Other Image URL",
            "format": "uri",
            "hidden": false,
            "pattern": "^(https?|s3)://",
            "editable": true,
            "examples": [
              "http://www.companyname.com/images/1250.other1.jpg"
            ],
            "description": "The URL for additional images of your product. These images will be shown on the detail page when the customer clicks through to see other views associated with the product."
          }
        },
        "additionalProperties": false
      },
      "title": "Other Product Image Locator 8",
      "examples": [
        "Feed"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "The attribute indicates the Other Product Image Locator 8 of the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "supplemental_condition_information": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [],
        "properties": {
          "cosmetic": {
            "enum": [
              "almost_no_sign_of_use",
              "highly_visible_sign_of_use",
              "light_sign_of_use",
              "moderately_visible_sign_of_use",
              "no_sign_of_use",
              "unknown"
            ],
            "type": "string",
            "title": "Cosmetic",
            "hidden": false,
            "editable": true,
            "examples": [
              "No Sign of Use"
            ],
            "enumNames": [
              "Almost No Sign Of Use",
              "Highly Visible Sign Of Use",
              "Light Sign Of Use",
              "Moderately Visible Sign Of Use",
              "No Sign Of Use",
              "Unknown"
            ],
            "description": "Provide the overall cosmetic condition of the non-new product."
          },
          "features": {
            "type": "array",
            "items": {
              "enum": [
                "green_refurbishment",
                "parts_inspected",
                "parts_replaced",
                "with_tags"
              ],
              "type": "string",
              "enumNames": [
                "Green Refurbishment",
                "Parts Inspected",
                "Parts Replaced",
                "With Tags"
              ]
            },
            "title": "Features",
            "hidden": false,
            "editable": true,
            "examples": [
              "Green Refurbishment"
            ],
            "maxItems": 10,
            "minItems": 1,
            "description": "Provide the refurbishment type of the non-new product."
          },
          "packaging": {
            "enum": [
              "amazon",
              "generic",
              "not_applicable",
              "oem_original",
              "oem_pre_owned"
            ],
            "type": "string",
            "title": "Packaging",
            "hidden": false,
            "editable": true,
            "examples": [
              "OEM Original"
            ],
            "enumNames": [
              "Amazon",
              "Generic",
              "Not Applicable",
              "OEM Original",
              "OEM Pre-Owned"
            ],
            "description": "Provide the packaging type of the non-new product"
          },
          "accessories": {
            "enum": [
              "generic",
              "not_applicable",
              "not_included",
              "oem"
            ],
            "type": "string",
            "title": "Accessories",
            "hidden": false,
            "editable": true,
            "examples": [
              "Generic"
            ],
            "enumNames": [
              "Generic",
              "Not Applicable",
              "Not Included",
              "OEM"
            ],
            "description": "Provide the type of accessory included in the non-new product."
          },
          "source_type": {
            "enum": [
              "as_is",
              "cpo",
              "no_data",
              "refurbished_amazon",
              "refurbished_oem",
              "refurbished_third_party",
              "returned_never_used",
              "returned_used"
            ],
            "type": "string",
            "title": "Source Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "Returned Never Used"
            ],
            "enumNames": [
              "As Is",
              "CPO",
              "No Data",
              "Refurbished Amazon",
              "Refurbished OEM",
              "Refurbished Third Party",
              "Returned Never Used",
              "Returned Used"
            ],
            "description": "Provide the information on how the non-new product was sourced."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "functional_condition": {
            "enum": [
              "fully_functional",
              "partly_functional",
              "unknown"
            ],
            "type": "string",
            "title": "Functional Condition",
            "hidden": false,
            "editable": true,
            "examples": [
              "Fully Functional"
            ],
            "enumNames": [
              "Fully Functional",
              "Partly Functional",
              "Unknown"
            ],
            "description": "Provide the functional condition of the non-new product."
          },
          "battery_life_percentage": {
            "enum": [
              "equal_to_or_less_than_60_percent",
              "greater_than_60_percent",
              "greater_than_70_percent",
              "greater_than_80_percent",
              "greater_than_90_percent",
              "no_battery"
            ],
            "type": "string",
            "title": "Battery Life Percentage",
            "hidden": false,
            "editable": true,
            "examples": [
              ">90%"
            ],
            "enumNames": [
              "=<60%",
              ">60%",
              ">70%",
              ">80%",
              ">90%",
              "No Battery"
            ],
            "description": "Provide the battery health information of the non-new product if it includes batteries."
          }
        },
        "additionalProperties": false
      },
      "title": "Supplemental Condition Information",
      "examples": [
        "iPhone 14, Open Box Never Used, OEM, Original, Greater than 90%, With Tags, Pristine, Fully Functional"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the additional condition information on the non-new product.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "supplier_declared_dg_hz_regulation": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              "ghs",
              "not_applicable",
              "other",
              "storage",
              "transportation",
              "unknown",
              "waste"
            ],
            "type": "string",
            "title": "Dangerous Goods Regulations",
            "hidden": false,
            "editable": true,
            "examples": [
              "GHS, Storage, Transportation"
            ],
            "enumNames": [
              "GHS",
              "Not Applicable",
              "Other",
              "Storage",
              "Transportation",
              "Unknown",
              "Waste"
            ],
            "description": "Provide the regulations that apply to the item if it is classified as a dangerous good, hazardous material, substance, or waste."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Dangerous Goods Regulations",
      "examples": [
        "GHS, Storage, Transportation"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide the regulations that apply to the item if it is classified as a dangerous good, hazardous material, substance, or waste.",
      "maxUniqueItems": 1000,
      "minUniqueItems": 1
    },
    "regulatory_compliance_certification": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "regulation_type",
          "value"
        ],
        "properties": {
          "value": {
            "type": "string",
            "title": "Regulatory Identification",
            "hidden": false,
            "editable": true,
            "examples": [
              "1AB1331-121A"
            ],
            "maxLength": 135,
            "minLength": 1,
            "description": "Provide the regulatory identification associated with the regulation type."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "regulation_type": {
            "enum": [
              "carb_eo",
              "cdpr_pest_id",
              "energy_star_unique_id",
              "certificate_of_conformity",
              "fda_510_k",
              "intertek_certificate_no",
              "national_organic_program_id",
              "tuv_certificate_no",
              "ul_cetrification_no",
              "wasda_pest_id"
            ],
            "type": "string",
            "title": "Compliance Regulation Type",
            "hidden": false,
            "editable": true,
            "examples": [
              "CDPR Pest Identification"
            ],
            "enumNames": [
              "CARB EO",
              "CDPR Pest Identification",
              "ENERGY STAR Unique ID",
              "EPA Certificate of Conformity (CoC)",
              "FDA 510(k) Number",
              "Intertek Certificate Number",
              "National Organic Program ID",
              "TUV Certificate Number",
              "UL Certificate Number",
              "WASDA Pest Identification"
            ],
            "description": "Select applicable regulation type"
          }
        },
        "additionalProperties": false
      },
      "title": "Regulatory Compliance Certification",
      "examples": [
        "FDA 510(k) Number,\r\nF2345G234"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "regulation_type"
      ],
      "description": "Provide any regulation that is relevant to the product as well as any required regulatory identications such as certification numbers.",
      "maxUniqueItems": 5,
      "minUniqueItems": 1
    },
    "externally_assigned_product_identifier": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "type",
          "value"
        ],
        "properties": {
          "type": {
            "enum": [
              "ean",
              "gtin",
              "upc"
            ],
            "type": "string",
            "title": "External Product ID Type",
            "hidden": false,
            "editable": false,
            "examples": [
              "UPC"
            ],
            "enumNames": [
              "EAN",
              "GTIN",
              "UPC"
            ],
            "description": "Select the type of external ID (barcode) that is being used to identify this product"
          },
          "value": {
            "type": "string",
            "title": "External Product ID",
            "hidden": false,
            "editable": false,
            "examples": [
              "714532191586"
            ],
            "description": "Provide the corresponding external product id value based on the type that was selected"
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "External Product ID",
      "examples": [
        "714532191586"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id",
        "type"
      ],
      "description": "Provide the external ID (barcode) type and corresponding value that is being used to identify the product",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "fcc_radio_frequency_emission_compliance": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "registration_status"
        ],
        "properties": {
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          },
          "registration_status": {
            "enum": [
              "fcc_supplier_declaration_of_conformity",
              "has_fcc_id",
              "fcc_incidental_radiator",
              "not_capable_emitting_rf_energy"
            ],
            "type": "string",
            "title": "Radio Frequency Emission & Authorization Status",
            "hidden": false,
            "editable": true,
            "examples": [
              "Product has FCC ID"
            ],
            "enumNames": [
              "Product has a Supplier's Declaration of Conformity (SDoC) with the FCC Rules",
              "Product has an FCC ID",
              "Product is an incidental radiator as defined by the FCC. It is not designed to intentionally use, generate or emit RF energy over 9 kHz. It does not require FCC RF equipment authorization",
              "Product not capable of emitting radio frequency energy"
            ],
            "description": "Indicate whether this product is capable of emitting radio frequency energy, and if so, what type of FCC RF equipment authorization this product has."
          },
          "identification_number": {
            "type": "string",
            "title": "FCC ID",
            "hidden": false,
            "editable": true,
            "examples": [
              "2AFZZ-XMSF10G"
            ],
            "maxLength": 100,
            "description": "If the device has an FCC ID, provide it."
          },
          "point_of_contact_name": {
            "type": "string",
            "title": "SDoC Contact Name",
            "hidden": false,
            "editable": true,
            "examples": [
              "John Doe"
            ],
            "maxLength": 100,
            "description": "If the device has a Supplier's Declaration of Conformity, provide the name of the point of contact for the Responsible Party, as defined by the FCC."
          },
          "point_of_contact_email": {
            "type": "string",
            "title": "SDoC Contact Email Address",
            "hidden": false,
            "editable": true,
            "examples": [
              "jdoe@example.eg"
            ],
            "maxLength": 300,
            "description": "If the device has an SDoC, provide an e-mail address (in this field) or a US phone number (in the next field) for the Responsible Party, as defined by the FCC. If you provide a phone number in the next field, you may enter \"N/A\" in this field."
          },
          "point_of_contact_address": {
            "type": "string",
            "title": "SDoC Contact US Mailing Address",
            "hidden": false,
            "editable": true,
            "examples": [
              "500 Oak Street\r\nChicago, IL 60707"
            ],
            "maxLength": 2500,
            "description": "If the device has a Supplier's Declaration of Conformity, provide a US mailing address for the Responsible Party, as defined by the FCC."
          },
          "point_of_contact_phone_number": {
            "type": "string",
            "title": "SDOC Contact US Phone Number",
            "hidden": false,
            "editable": true,
            "examples": [
              "777-767-1000"
            ],
            "maxLength": 100,
            "description": "If the device has an SDoC, provide a US phone number (in this field) or an e-mail address (in the prior field) for the Responsible Party, as defined by the FCC. If you provide an e-mail address in the prior field, you may enter \"N/A\" in this field."
          }
        },
        "additionalProperties": false
      },
      "title": "FCC Radio Frequency Emission Compliance",
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Provide details on compliance to FCC regulations for products that may emit radio frequencies.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    },
    "supplier_declared_has_product_identifier_exemption": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "value"
        ],
        "properties": {
          "value": {
            "enum": [
              false,
              true
            ],
            "type": "boolean",
            "title": "Is exempt from supplier declared external product identifier",
            "hidden": false,
            "editable": true,
            "examples": [
              "Yes, No"
            ],
            "enumNames": [
              "No",
              "Yes"
            ],
            "description": "Please specify if the product is exempt from supplier declared external product identifiers."
          },
          "marketplace_id": {
            "$ref": "#/$defs/marketplace_id"
          }
        },
        "additionalProperties": false
      },
      "title": "Is exempt from a supplier declared external identifier",
      "examples": [
        "Y, N"
      ],
      "minItems": 1,
      "selectors": [
        "marketplace_id"
      ],
      "description": "Please specify if the product is exempt from supplier declared external product identifiers.",
      "maxUniqueItems": 1,
      "minUniqueItems": 1
    }
  },
  "additionalProperties": false
}
